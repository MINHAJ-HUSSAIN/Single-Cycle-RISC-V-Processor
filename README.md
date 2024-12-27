# Single-Cycle RISC-V Processor

This repository provides a step-by-step guide to developing a single-cycle RISC-V processor. The processor executes each instruction within a single clock cycle and integrates Control and Status Registers (CSR) for efficient system-level control and exception management. The CSR trap mechanism is hardwired to ensure reliable exception handling.

# Tools and Requirements

Before starting, ensure the following tools are installed:

### SystemVerilog:
A hardware description language for designing the processor.

### Code Editor (e.g., VS Code):
Recommended for managing code files. Install SystemVerilog extensions for improved functionality.

### GTKWave:
For waveform visualization during simulations. Some features may require Multisim.

# Simulation Tools:
Use ModelSim, Quartus, or Vivado to compile and simulate the design.

# Commands for Compilation and Simulation

Run the following commands to compile, simulate, and analyze the processor:

### Compile SystemVerilog Design Files:

vlog -work work *.sv

### Simulate the Testbench:

vsim -c processor_testbench -do "run -all"

### View Waveforms:

gtkwave output_waveform.vcd

# Workflow Overview

1. Setting Up the Project

Open the project folder using your code editor (e.g., VS Code).

Install SystemVerilog extensions for enhanced editing capabilities.

2. Compiling the Design

Use a simulator such as ModelSim or Vivado to compile the SystemVerilog files.

Ensure that all dependencies are resolved before proceeding.

3. Running Simulations

Execute the testbench to verify the processor’s behavior in various scenarios.

4. Analyzing Results

Load the .vcd file into GTKWave to observe signal transitions and debug the design.

Use Multisim if additional debugging features are required.

5. Enhancing the Processor

Add new instructions to extend the processor’s functionality.

Test CSR features by simulating exception scenarios and analyzing the response.

# Key Features

### Single-Cycle Execution:
Simplifies control logic by completing each instruction in one clock cycle.

### CSR Integration:
Provides robust system control and efficient exception management with a hardwired mechanism.

### Customizable Design:
Expand the processor by implementing additional RISC-V instructions and testing advanced features.
