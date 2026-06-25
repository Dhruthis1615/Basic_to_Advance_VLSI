# Task 2: Verilog HDL Implementation of Basic Logic Gates, Half Adder and Full Adder

## 📖 Overview

This task focuses on implementing fundamental digital circuits using **Verilog HDL**. The objective is to understand how hardware can be described using a Hardware Description Language (HDL), simulate the designs, and verify their functionality through waveform analysis.

The circuits were simulated using **Icarus Verilog**, and the generated waveforms were analyzed using **GTKWave** to ensure the outputs matched the expected Boolean logic and truth tables.

---

## 🎯 Objectives

- Learn the fundamentals of Verilog HDL.
- Implement basic logic gates using Verilog.
- Develop testbenches for functional verification.
- Simulate digital circuits using Icarus Verilog.
- Analyze waveforms using GTKWave.
- Implement and verify Half Adder and Full Adder circuits.

---

## 🛠️ Tools Used

- Verilog HDL
- Icarus Verilog
- GTKWave
- Ubuntu (WSL)

---

## 📂 Project Structure

```
.
├── logic_gates.v
├── tb_logic_gates.v
├── half_adder.v
├── tb_half_adder.v
├── full_adder.v
├── tb_full_adder.v
├── waveforms/
└── README.md
```

---

## ✅ Implemented Modules

### Basic Logic Gates

- AND Gate
- OR Gate
- NOT Gate
- NAND Gate
- NOR Gate
- XOR Gate

Each module includes:
- Verilog implementation
- Testbench
- Waveform verification

---

### Half Adder

Implements binary addition of two inputs.

**Boolean Expressions**

```
SUM   = A ^ B
CARRY = A & B
```

Includes:
- Verilog module
- Testbench
- Waveform verification

---

### Full Adder

Implements binary addition of three inputs.

**Boolean Expressions**

```
SUM   = A ^ B ^ Cin
CARRY = (A & B) | (B & Cin) | (A & Cin)
```

Includes:
- Verilog module
- Testbench
- Waveform verification

---

## ▶️ Running the Simulations

### Compile

```bash
iverilog -o logic_gates logic_gates.v tb_logic_gates.v
iverilog -o half_adder half_adder.v tb_half_adder.v
iverilog -o full_adder full_adder.v tb_full_adder.v
```

### Run

```bash
vvp logic_gates
vvp half_adder
vvp full_adder
```

### View Waveforms

```bash
gtkwave logic_gates.vcd
gtkwave half_adder.vcd
gtkwave full_adder.vcd
```

---

## 📊 Results

- Successfully implemented all six basic logic gates in Verilog.
- Verified Half Adder and Full Adder functionality using testbenches.
- Generated waveform outputs using GTKWave.
- Simulation results matched the expected Boolean expressions and truth tables.

---

## 🚀 Applications

- FPGA Design
- ASIC Design
- Arithmetic Logic Units (ALUs)
- Processors and Microcontrollers
- Digital Signal Processing
- VLSI Design and Verification

---

## 📚 References

1. Icarus Verilog Documentation
2. GTKWave User Guide
3. Verilog HDL – Samir Palnitkar
4. Digital Design – Morris Mano
5. IEEE Verilog HDL Standard

---

## 👩‍💻 Author

**Dhruthi S**  
Electronics and Communication Engineering  
Dayananda Sagar Academy of Technology and Management (DSATM)

**VLSI Internship – Maincrafts Technology**
