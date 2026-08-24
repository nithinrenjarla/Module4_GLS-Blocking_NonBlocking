# Module4_GLS-Blocking_NonBlocking
MODLE 4: Blocking vs Non-Blocking Assignments-Simulation Mismatch using Verilog, Icarus Verilog,GTKWave, Yosys and SKY130

# Introduction
Blocking (=) and non-blocking (<=) assignments are fundamental concepts in Verilog HDL. They determine how statements are executed within procedural blocks.
Proper use of these assignments is essential for designing reliable and synthesizable digital circuits. This module demonstrates the implementation of multiplexers, the behavior of blocking and non-blocking assignments, and common synthesis–simulation mismatch scenarios.
The designs are simulated using Icarus Verilog, analyzed using GTKWave, synthesized using Yosys, and mapped to the SKY130 standard-cell library.
# Objectives
To understand the difference between blocking (=) and non-blocking (<=) assignments.
To study the causes of synthesis–simulation mismatch.
To design and simulate multiplexer circuits using Verilog.
To analyze the behavior of blocking assignments through RTL simulation.
To verify circuit functionality using Icarus Verilog and GTKWave.
To synthesize RTL designs using Yosys.
To map synthesized circuits to the SKY130 standard-cell library.
To compare RTL simulation results with synthesized results.

# Tools and Technologies Used
| Tool / Technology |Purpose |
|---|---|
| Verilog HDL |RTL Design |
| Icarus Verilog | Compilation and Simulation |
| GTKWave | Waveform Analysis |
| Yosys | RTL Synthesis |
| SKY130 Standard Cell Library | Technology Mapping |
| Linux Terminal | Command Execution |
| gVim | Verilog Editing |

# Table of Contents
1. RTL Simulation of a 2×1 Multiplexer
2. Technology Mapping of the Multiplexer
3. Functional Verification Using Simulation Waveform
4. Analysis of an Incorrect Multiplexer Design
5. Verification of Bad Multiplexer Behavior
6. Simulation of Blocking Assignment Behavior
7. Synthesis of Blocking Assignment Circuit
8. Blocking Assignment Using Previous Value
9. Overall Result
10. Conclusion

# 1.RTL Simulation of a 2×1 Multiplexer
# Overview
A 2×1 multiplexer was implemented using the Verilog ternary operator to understand combinational logic design. The RTL design was simulated using Icarus Verilog, and the output waveform was verified using GTKWave. The experiment demonstrates how the output changes based on the select signal and validates the functional correctness of the multiplexer before synthesis.

# Simulation Commands
```verilog
iverilog -o mux ternary_operator_mux.v tb_ternary_operator_mux.v

gtkwave ternary_operator_mux.vcd
```
