# RV32I Assembler & Simulator (Custom ISA Project) 🧠🛠️

This project implements a custom **two-pass assembler** and a **cycle-accurate simulator** for a subset of the **RV32I (RISC-V 32-bit integer)** instruction set architecture. It includes full support for label resolution, binary instruction encoding, register/memory emulation, and bonus support for extended opcodes.

---

## 📌 Project Overview

As part of a system programming assignment at IIIT-Delhi, we designed and built:
- A fully functional assembler for converting `.s` files into 32-bit binary `.mc` files
- A simulator to execute these binary instructions and track all register/memory state
- Support for custom instructions: `mul`, `rst`, `halt`, `rvrs` (bonus Q3)

---

## 🧠 Key Features

### 🔹 Assembler
- Parses labels, ABI-compliant register names, and instructions
- Implements two-pass architecture with:
  - Label offset resolution for `beq`, `jal`, etc.
  - Error handling (invalid register, immediate bounds, missing virtual halt)
- Outputs one 32-bit binary instruction per line to `stdout`
- Handles:
  - `ErrorGen` cases (manual check)
  - `simpleBin` and `hardGen` binary generation

### 🔹 Simulator
- Simulates execution of each instruction from `.mc` file
- Tracks 32 registers (`x0` to `x31`) and 32 memory addresses (32 × 32-bit)
- Prints register values after **every instruction execution**
- Dumps full memory contents after **virtual halt**
- Format:
