# Task 3 – Verilog HDL Implementation of Sequential Circuits

## 📖 Overview

This task focuses on the implementation and simulation of fundamental **sequential circuits** using **Verilog HDL**. Unlike combinational circuits, sequential circuits depend on both the current inputs and previous states, making them the building blocks of registers, counters, processors, and memory systems.

Each circuit was designed in Verilog HDL, functionally verified using **Icarus Verilog**, and analyzed through **GTKWave** to validate its behavior.

---

## 🎯 Objectives

- Design sequential circuits using Verilog HDL
- Implement a D Flip-Flop
- Implement a JK Flip-Flop
- Implement a 4-bit Register
- Implement a 4-bit Binary Counter
- Develop testbenches for functional verification
- Analyze simulation waveforms using GTKWave

---

## 🛠️ Tools Used

- Verilog HDL
- Icarus Verilog
- GTKWave
- Ubuntu (WSL)

---

## 📂 Repository Structure

```
Task 3
│
├── D Flip-Flop
│   ├── d_flipflop.v
│   ├── tb_d_flipflop.v
│   ├── d_flipflop.vcd
│   └── waveform.png
│
├── JK Flip-Flop
│   ├── jk_flipflop.v
│   ├── tb_jk_flipflop.v
│   ├── jk_flipflop.vcd
│   └── waveform.png
│
├── 4-bit Register
│   ├── register4.v
│   ├── tb_register4.v
│   ├── register4.vcd
│   └── waveform.png
│
├── 4-bit Binary Counter
│   ├── counter4.v
│   ├── tb_counter4.v
│   ├── counter4.vcd
│   └── waveform.png
│
└── README.md
```

---

# 📚 Implemented Sequential Circuits

## 1️⃣ D Flip-Flop

The **D (Data) Flip-Flop** is a positive-edge-triggered sequential circuit that stores a single bit of data. The output updates only on the rising edge of the clock.

### Features

- Positive-edge triggered
- Single-bit data storage
- Synchronous operation

### Files

- `d_flipflop.v`
- `tb_d_flipflop.v`

### Simulation Waveform

> Replace with your image path

```md
![D Flip-Flop Waveform](D%20Flip-Flop/waveform.png)
```

### Observation

The output successfully captures the input value on every positive edge of the clock, confirming correct sequential behavior.

---

## 2️⃣ JK Flip-Flop

The **JK Flip-Flop** removes the invalid state found in SR Flip-Flops and supports four different operations depending on the values of J and K.

### Truth Table

| J | K | Operation |
|:-:|:-:|-----------|
| 0 | 0 | Hold |
| 0 | 1 | Reset |
| 1 | 0 | Set |
| 1 | 1 | Toggle |

### Files

- `jk_flipflop.v`
- `tb_jk_flipflop.v`

### Simulation Waveform

```md
![JK Flip-Flop Waveform](JK%20Flip-Flop/waveform.png)
```

### Observation

Simulation verifies all four operations—Hold, Reset, Set, and Toggle—with output changing only on the positive edge of the clock.

---

## 3️⃣ 4-bit Register

A **4-bit Register** stores four bits of data simultaneously and updates its output on the rising edge of the clock.

### Features

- Parallel 4-bit input
- Parallel 4-bit output
- Positive-edge triggered

### Files

- `register4.v`
- `tb_register4.v`

### Simulation Waveform

```md
![4-bit Register Waveform](4-bit%20Register/waveform.png)
```

### Observation

The register correctly stores and transfers each 4-bit input value on every positive clock edge.

---

## 4️⃣ 4-bit Binary Counter

The **4-bit Binary Counter** increments its value on every positive edge of the clock.

### Features

- Positive-edge triggered
- Counts from **0000** to **1111**
- Automatically rolls over to **0000**

### Files

- `counter4.v`
- `tb_counter4.v`

### Simulation Waveform

```md
![4-bit Counter Waveform](4-bit%20Binary%20Counter/waveform.png)
```

### Observation

The counter increments sequentially from **0 to 15** before rolling over, demonstrating correct counting functionality.

---

# ▶️ Running the Simulation

Compile the Verilog design:

```bash
iverilog -o output design.v testbench.v
```

Execute the simulation:

```bash
vvp output
```

Open the generated waveform:

```bash
gtkwave waveform.vcd
```

Replace:

- `design.v` with the module file
- `testbench.v` with the corresponding testbench
- `waveform.vcd` with the generated waveform file

---

# ✅ Results

All sequential circuits were successfully implemented and verified using dedicated testbenches.

Simulation results confirmed:

- ✔️ Correct positive-edge-triggered operation
- ✔️ Accurate sequential data storage
- ✔️ Proper JK Flip-Flop functionality
- ✔️ Correct binary counting sequence
- ✔️ Expected waveform outputs in GTKWave

---

# 🚀 Applications

- FPGA Design
- ASIC Design
- Digital Registers
- Digital Counters
- Memory Elements
- Embedded Systems
- Processor Design
- VLSI Design & Verification

---

# 📖 Learning Outcomes

Through this task, the following concepts were learned:

- Sequential logic design using Verilog HDL
- RTL coding practices
- Testbench development
- Functional simulation using Icarus Verilog
- Waveform analysis using GTKWave
- Verification of clock-driven digital circuits

---

# 📚 References

1. Icarus Verilog Documentation
2. GTKWave Documentation
3. **Verilog HDL** — Samir Palnitkar
4. **Digital Design** — Morris Mano
5. IEEE Verilog HDL Standard

---

## 👩‍💻 Author

**Dhruthi S**

Electronics and Communication Engineering  
Dayananda Sagar Academy of Technology and Management (DSATM)

**Internship Domain:** VLSI Design
