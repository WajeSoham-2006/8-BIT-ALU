
# 8-bit ALU using VHDL

## About the Project

I built this 8-bit Arithmetic Logic Unit (ALU) using VHDL in Xilinx Vivado
as a way to learn digital design and hardware description languages.

The ALU takes two 8-bit inputs, A and B, and performs different operations
depending on the 4-bit selection input (opcode). The result is available
through an 8-bit output, along with a carry/borrow flag and a zero flag.

I also created a testbench to check the operations and observe their
outputs using Vivado's behavioral simulation.

## Operations

The ALU currently supports the following operations:

| Opcode | Operation |
|--------|-----------|
| 0000 | Addition (A + B) |
| 0001 | Subtraction (A - B) |
| 0010 | Bitwise OR |
| 0011 | Bitwise AND |
| 0100 | Bitwise XOR |
| 0101 | Bitwise NOT of A |
| 0110 | Bitwise NOT of B |
| 0111 | Left shift of A by 1 bit |
| 1000 | Right shift of A by 1 bit |

## Inputs and Outputs

- **A:** First 8-bit input operand.
- **B:** Second 8-bit input operand.
- **S:** 4-bit opcode used to select the operation.
- **Y:** 8-bit output containing the operation's result.
- **C:** Flag used to indicate carry during addition or borrow during subtraction.
- **Flag:** Zero flag, set when the result is zero.

## Tools Used

- VHDL
- Xilinx Vivado 2026.1
- Vivado Behavioral Simulation

## Testing

I used a VHDL testbench to apply different input combinations and
opcodes to the ALU. I then checked the output values and flags
in the simulation waveform.

This helped me understand how the ALU responds to different operations
and how to verify a digital design through simulation.

## What I Learned

While working on this project, I learned how to:

- Write a VHDL entity and architecture.
- Use a case statement to select operations using an opcode.
- Perform arithmetic and bitwise operations.
- Use the `numeric_std` library for unsigned arithmetic.
- Handle carry and borrow conditions.
- Implement left and right shift operations.
- Create a testbench and analyse simulation waveforms.

## Future Scope

I plan to improve the design further as I learn more about VHDL,
digital electronics, and FPGA design.
