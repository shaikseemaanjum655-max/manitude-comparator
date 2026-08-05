# 4-bit Magnitude Comparator using Verilog

## Overview

This project implements a **4-bit Magnitude Comparator** using Verilog HDL.

A magnitude comparator compares two 4-bit binary numbers and determines whether:

- A is greater than B
- A is less than B
- A is equal to B

## Inputs

- `A[3:0]` - First 4-bit binary number
- `B[3:0]` - Second 4-bit binary number

## Outputs

- `A_greater` - High when A > B
- `A_less` - High when A < B
- `A_equal` - High when A = B

## Truth Table

| Condition | A_greater | A_less | A_equal |
|-----------|-----------|--------|---------|
| A > B | 1 | 0 | 0 |
| A < B | 0 | 1 | 0 |
| A = B | 0 | 0 | 1 |

## Project Structure

```
4bit-magnitude-comparator-verilog/
├── src/
├── tb/
├── sim/
├── images/
└── README.md
```

## Simulation

Compile:

```bash
iverilog -o comparator src/magnitude_comparator.v tb/magnitude_comparator_tb.v
```

Run:

```bash
vvp comparator
```

Open waveform:

```bash
gtkwave magnitude_comparator.vcd
```

## Applications

- Digital processors
- Sorting circuits
- Address comparison
- Control systems
- FPGA and ASIC designs

## License

MIT License