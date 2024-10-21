- [Registers](#registers)
    - [Status Register](#status-register)
    - [Control Register](#control-register)
- [Memory](#memory)
- [Instructions](#instructions)
  - [Instruction Format](#instruction-format)

# Registers
Registers are 32-bit wide. There are 11 general purpose registers, named r0-r11 as well as some registers with special functions as shown in the table below.

| Name    | Purpose                |
|---------|------------------------|
| r0 - r11| general purpose        |
| sp      | stack pointer          |
| ra      | return address pointer |
| pc      | program counter        |
| st      | status register        |
| ct      | control register       |

### Status Register
Will be used to check various conditions of cpu

### Control Register
Will be used to set various funtionalities of cpu

# Memory
The are 2<sup>32</sup> memory-addresses, ranging from 0 to 2<sup>32</sup> - 1, where each address adresses one byte (8 bit) in memory. This allows for up to 4 GiB of memory.

# Instructions
The AU32-ISA is a load-store-architecture. This means, that the only operations able to interact with memory are operations either storing contents of a register into memory or loading values from memory into a register.

## Instruction Format
Instructions are of a fixed length of 32 bits. 