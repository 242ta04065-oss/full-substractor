# Full Subtractor using Verilog

## Overview

This project implements a **1-bit Full Subtractor** using Verilog HDL. A Full Subtractor is a combinational logic circuit that subtracts two binary bits along with a borrow input. It generates two outputs: **Difference (D)** and **Borrow Out (Bout)**.

This project includes:

* Verilog implementation of a Full Subtractor
* Testbench for functional verification
* Simulation results
* Truth table
* Waveform screenshots

## Truth Table

| A | B | Bin | Difference | Borrow Out |
| - | - | --- | ---------- | ---------- |
| 0 | 0 | 0   | 0          | 0          |
| 0 | 0 | 1   | 1          | 1          |
| 0 | 1 | 0   | 1          | 1          |
| 0 | 1 | 1   | 0          | 1          |
| 1 | 0 | 0   | 1          | 0          |
| 1 | 0 | 1   | 0          | 0          |
| 1 | 1 | 0   | 0          | 0          |
| 1 | 1 | 1   | 1          | 1          |

## Boolean Expressions

Difference = A ⊕ B ⊕ Bin

Borrow Out = (~A & B) | (~A & Bin) | (B & Bin)

## Files

* `full_subtractor.v` – Verilog implementation
* `full_subtractor_tb.v` – Testbench
* `simulation/` – Waveform and simulation output

## Simulation

The testbench verifies all eight possible input combinations. The generated waveform confirms the correct Difference and Borrow Out outputs for every case.

## Tools Used

* Verilog HDL
* ModelSim / Vivado / Icarus Verilog
* GTKWave (optional)

## Applications

* Arithmetic Logic Units (ALUs)
* Digital processors
* Embedded systems
* Computer architecture
* Digital electronics education

## Author

sravani
