# 🧮 8-Bit ALU Simulation (Logisim)

## 📌 Overview

This project presents the design and simulation of an **8-bit Arithmetic Logic Unit (ALU)** using digital logic components in Logisim.

The ALU performs arithmetic and logical operations on two 8-bit inputs based on a control signal. This project demonstrates fundamental digital design principles used in CPU architecture.

---

## 🎯 Project Objectives

- Design an 8-bit ALU using combinational logic circuits
- Implement arithmetic and logical operations
- Understand CPU datapath fundamentals
- Simulate and verify ALU functionality

---

## 🧠 What is an ALU?

The **Arithmetic Logic Unit (ALU)** is a core component of a processor responsible for performing:

- Arithmetic operations (Addition, Subtraction)
- Logical operations (AND, OR, NOT, XOR)
- Bitwise operations
- Comparison operations

It is one of the most critical building blocks of modern CPUs.

---

## ⚙️ Implemented Operations

Depending on the control signal (Opcode), the ALU performs:

| Control Signal | Operation |
|---------------|------------|
| 000 | A + B |
| 001 | A - B |
| 010 | A AND B |
| 011 | A OR B |
| 100 | A XOR B |
| 101 | NOT A |
| 110 | A << 1 (Shift Left) |
| 111 | A >> 1 (Shift Right) |

---

## ➕ Arithmetic Foundation

The addition operation is based on the Full Adder equation:

Sum:

S = A ⊕ B ⊕ Cin  

Carry-out:

Cout = (A · B) + (Cin · (A ⊕ B))

The 8-bit adder is constructed using 8 cascaded full adders.

---

## 🏗 Design Architecture

The ALU consists of:

- 8-bit ripple carry adder
- Logic gates (AND, OR, XOR, NOT)
- Multiplexers for operation selection
- Control logic input (Opcode)
- 8-bit input buses (A and B)
- 8-bit output bus
- Carry and Zero flags

---

## 📊 Flags Implemented

- Carry Flag (C)
- Zero Flag (Z)
- (Optional) Overflow Flag (V)

These flags are essential in processor design for branching and decision-making.

---

## 🔬 Simulation Tool

The circuit was designed and simulated using:

Logisim / Logisim Evolution

File included:

8bit ALU simulation.circ

---

## 🏆 Learning Outcomes

- Digital logic circuit design
- Combinational circuit analysis
- Binary arithmetic implementation
- CPU datapath understanding
- Hardware-level problem solving

---

## 🚀 Future Improvements

- Add signed arithmetic support
- Implement overflow detection
- Design 16-bit version
- Integrate into full CPU architecture
- Implement using Verilog (FPGA-ready)

---

## 👨‍💻 Author

Mohammed Faris Al-khammash  
Computer Engineering Student  

---

## 📄 License

Educational and academic use only.
