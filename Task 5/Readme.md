# Verilog HDL Implementation of Datapath, ALU, and Memory Components (RAM/ROM)

## Overview

This project demonstrates the implementation and functional verification of fundamental datapath and memory components using **Verilog HDL**. The modules were designed, simulated, and verified using **Icarus Verilog** and **GTKWave**.

The project includes the implementation of:

- Arithmetic Logic Unit (ALU)
- Register File
- Random Access Memory (RAM)
- Read-Only Memory (ROM)
- Simple Datapath

These components form the core building blocks of digital processors, embedded systems, FPGA designs, and ASIC implementations.

---

## Objectives

- Design datapath components using Verilog HDL.
- Implement a 4-bit Arithmetic Logic Unit (ALU).
- Design a Register File with read and write operations.
- Implement Random Access Memory (RAM).
- Implement Read-Only Memory (ROM).
- Integrate the ALU into a simple datapath.
- Perform functional simulation using Icarus Verilog.
- Verify outputs using GTKWave waveform analysis.

---

## Tools Used

- Verilog HDL
- Icarus Verilog
- GTKWave
- Ubuntu (WSL)

---

# Project Structure

```
.
├── alu.v
├── tb_alu.v
├── register_file.v
├── tb_register_file.v
├── ram.v
├── tb_ram.v
├── rom.v
├── tb_rom.v
├── datapath.v
├── tb_datapath.v
└── README.md
```

---

# Modules Implemented

## 1. Arithmetic Logic Unit (ALU)

A 4-bit ALU capable of performing arithmetic and logical operations based on a 3-bit select signal.

### Operations Supported

| Select | Operation |
|---------|-----------|
| 000 | Addition |
| 001 | Subtraction |
| 010 | AND |
| 011 | OR |
| 100 | XOR |

### Verification

The ALU was simulated successfully, and waveform analysis confirmed correct execution of all arithmetic and logical operations.

---

## 2. Register File

A 4-register register file with:

- Synchronous write operation
- Asynchronous read operation
- 4-bit data width
- 2-bit addressing

### Features

- Positive-edge triggered write
- Immediate read access
- Register initialization to zero

### Verification

Simulation verified correct write and read functionality for different register addresses.

---

## 3. Random Access Memory (RAM)

A 4×4 RAM supporting:

- Synchronous write
- Asynchronous read

### Features

- 4 memory locations
- 4-bit data width
- Write Enable (WE) control
- Positive-edge clocked write

### Verification

Waveform analysis confirmed successful storage and retrieval of data from memory locations.

---

## 4. Read-Only Memory (ROM)

A 4×4 ROM initialized with predefined data values.

### Stored Data

| Address | Data |
|---------|------|
| 00 | 0001 |
| 01 | 0010 |
| 10 | 0100 |
| 11 | 1000 |

### Verification

Simulation verified that each address correctly outputs its predefined value without requiring any write operation.

---

## 5. Datapath

A simple datapath integrating the ALU.

### Features

- Accepts two operands
- Uses ALU as processing element
- Performs arithmetic and logical operations
- Produces output based on the select signal

### Verification

Simulation confirmed proper data transfer between operands and the ALU, producing the expected outputs.

---

# Simulation

Each module was verified using its dedicated testbench.

Simulation steps:

1. Compile the Verilog files using Icarus Verilog.
2. Generate the VCD waveform.
3. Open the waveform using GTKWave.
4. Verify the functionality of each module.

---

# Results

All modules were successfully implemented and verified.

The following components functioned correctly:

- Arithmetic Logic Unit (ALU)
- Register File
- Random Access Memory (RAM)
- Read-Only Memory (ROM)
- Datapath

Waveform analysis using GTKWave validated the expected functionality of every module.

---

# Applications

- FPGA Design
- ASIC Design
- Processor Datapath Design
- Embedded Systems
- Digital Signal Processing (DSP)
- Computer Architecture
- Memory Systems
- VLSI Design and Verification

---

# Conclusion

The ALU, Register File, RAM, ROM, and Datapath were successfully implemented using Verilog HDL. Functional verification using Icarus Verilog and GTKWave confirmed the correct operation of all modules. This project provides practical experience in designing, simulating, and verifying essential datapath and memory components used in digital systems and VLSI design.

---

# References

1. Icarus Verilog Documentation
2. GTKWave User Guide
3. *Verilog HDL* – Samir Palnitkar
4. *Digital Design* – Morris Mano
5. IEEE Verilog HDL Standard
