# Logisim Simulation using SimpleRiscISA

**ECE303 – Computer Organization & Design Project**

---

## 📌 Project Overview

This project demonstrates the implementation and simulation of a simple **RISC-based Instruction Set Architecture (SimpleRiscISA)** using **Logisim**. The main objective is to execute a memory-based summation program and verify its correctness through simulation.

The project focuses on understanding:

* Instruction execution in a RISC processor
* Memory addressing and data path behavior
* Assembly-level programming and encoding
* End-to-end flow from assembly code to machine-level execution

---

## 🧠 Problem Statement

**MEMORY_SUM**

An integer **N** is stored at memory location **0x1000**. The task is to calculate the sum of **N integers** stored at **continuous memory locations starting from 0x1001**.

The program should:

1. Read the value of **N** from memory
2. Iteratively access the next **N** memory locations
3. Accumulate the sum
4. Store or display the final result

The design is demonstrated for **various values of N** to validate correctness.

---

## 🛠️ Tools & Technologies Used

* **Logisim** – for processor and datapath simulation
* **SimpleRiscISA** – custom/simple RISC instruction set architecture
* **Assembly Language** – program implementation
* **GitHub** – version control and project hosting

---

## 📂 Repository Structure

```
Logisim_simulation_using_SimpleRiscISA/
│
├── README.md          # Project documentation
├── code_final.s       # Final assembly program for MEMORY_SUM
├── encode_final.s     # Instruction encoding logic
├── instr_hex.dat      # Hexadecimal machine code used in Logisim
```

---

## ⚙️ Implementation Flow

1. **Assembly Program (`code_final.s`)**

   * Written using the **SimpleRiscISA** instruction set
   * Implements the MEMORY_SUM logic (loading N, looping through memory, accumulation)
   * **Correctness verified** using the *official utility web tool provided by the course instructor*

2. **Instruction Encoding (`encode_final.s`)**

   * Contains the **`.encode` format** of the above SimpleRiscISA assembly program
   * Encoding was generated and verified using the same utility web tool
   * Aids in understanding how assembly instructions map to machine-level representation

3. **Machine Code (`instr_hex.dat`)**

   * Final encoded instructions converted into **hexadecimal format**
   * This file is directly loaded into **Logisim instruction memory**

4. **Logisim Simulation & Verification**

   * The `.dat` file is used to simulate program execution in Logisim
   * Program execution is observed step-by-step
   * **Register contents are monitored** to verify correct data loading, looping behavior, and final sum computation

This flow ensures correctness at every stage: assembly → encoding → machine code → hardware-level simulation.

---

## ✅ Verification & Results

* The program was tested with **multiple values of N**
* Correct summation observed for all test cases
* Confirms proper functioning of:

  * Instruction fetch & decode
  * Memory addressing
  * ALU operations
  * Control flow (loop execution)

---

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience in:

* Designing and simulating a basic RISC processor
* Writing and debugging assembly programs
* Understanding instruction encoding and execution
* Bridging theoretical concepts of computer organization with practical implementation

---

## 👤 Author

**Jaswanth (ECE’27)**
Computer Organization & Design Project

---

⭐ If you find this project useful, feel free to star the repository!

