# VLSI Task 1 – Digital Logic Gates and Combinational Circuits

This repository contains the implementation and simulation of fundamental digital logic gates and basic combinational circuits as part of the **VLSI Design Internship** at **Maincrafts Technology**.

## 📌 Overview

This project introduces the fundamentals of digital logic design by implementing and verifying:

- Basic Logic Gates
- Half Adder
- Full Adder

All circuits were designed and simulated using **CircuitVerse**, and their outputs were verified using truth tables.

---

## 🎯 Objectives

- Understand the fundamentals of VLSI technology.
- Study the VLSI design flow.
- Learn the operation of basic logic gates.
- Verify logic gate functionality using truth tables.
- Design and simulate Half Adder circuits.
- Implement and verify Full Adder circuits.

---

## 🛠️ VLSI Design Flow

```
System Specification
        ↓
Architecture Design
        ↓
RTL Design
        ↓
Functional Verification
        ↓
Logic Synthesis
        ↓
Physical Design
        ↓
Timing Analysis
        ↓
Fabrication
        ↓
Testing & Validation
```

---

## 📂 Implemented Circuits

### Basic Logic Gates

- AND Gate
- OR Gate
- NOT Gate
- NAND Gate
- NOR Gate
- XOR Gate

Each implementation includes:

- Circuit Diagram
- Boolean Expression
- Truth Table
- Simulation Results
- Observation

---

### Half Adder

The Half Adder performs the addition of two binary inputs.

**Outputs**
- Sum
- Carry

**Boolean Expressions**

```
Sum = A ⊕ B
Carry = A · B
```

---

### Full Adder

The Full Adder performs the addition of three binary inputs.

**Inputs**
- A
- B
- Carry In (Cin)

**Outputs**
- Sum
- Carry Out (Cout)

**Boolean Expressions**

```
Sum  = A ⊕ B ⊕ Cin
Cout = (A · B) + (Cin · (A ⊕ B))
```

---

## 💻 Software Used

- CircuitVerse

---

## ✅ Results

- Successfully designed and simulated all basic logic gates.
- Verified the functionality using truth tables.
- Successfully implemented Half Adder and Full Adder circuits.
- Simulation outputs matched the expected theoretical results.

---

## 🚀 Applications

### Logic Gates
- Digital electronic systems
- Processors and microcontrollers
- Control and decision-making circuits

### Half Adder
- Binary addition
- Arithmetic circuits
- Digital calculators

### Full Adder
- Multi-bit binary addition
- Arithmetic Logic Units (ALUs)
- CPUs and processors

---

## 📖 References

1. CircuitVerse Digital Logic Simulator
2. Digital Electronics – M. Morris Mano
3. Fundamentals of Digital Logic Design

---

## 👩‍💻 Author

**Dhruthi S**

Department of Electronics and Communication Engineering (ECE)

Dayananda Sagar Academy of Technology and Management (DSATM)

VLSI Design Internship – Maincrafts Technology
