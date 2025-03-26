# ➕ Half Adder (1-Bit Binary Adder)

## 🧠 Overview
The **Half Adder** is a fundamental digital circuit that adds **two 1-bit binary numbers** — inputs `A` and `B`. It produces two outputs:

- **Sum**: The result of the addition
- **Carry**: A bit that represents overflow when both inputs are 1

The Half Adder is called "half" because it does **not handle a carry-in** from a previous addition — for that, we'll need a **Full Adder**. This circuit is a building block for more complex arithmetic units like multi-bit adders and ALUs.

---

## 🔢 Truth Table

| A | B | Sum | Carry |
|---|---|-----|--------|
| 0 | 0 |  0  |   0    |
| 0 | 1 |  1  |   0    |
| 1 | 0 |  1  |   0    |
| 1 | 1 |  0  |   1    |

---

## ⚖️ Logic Expression

- **Sum = A XOR B**
- **Carry = A AND B**

This means the Half Adder can be built using:
- One **XOR gate** for the sum
- One **AND gate** for the carry

---

## ♻️ Gate Implementation Using NANDs
To build a Half Adder using only **NAND gates**:

1. Build an **XOR gate** using 4 NAND gates (see XOR Gate section)
2. Build an **AND gate** using 2 NAND gates:
   - `A AND B = NOT(A NAND B)`

Total: **6 NAND gates** minimum

---

## 📄 What I Learned
- How a Half Adder performs 1-bit binary addition
- XOR handles the **Sum** output, while AND handles the **Carry**
- How logic gates compose to perform real arithmetic
- Half Adders are the **first step** in building adders for CPUs and ALUs

---

## 🔧 Why It Matters
The Half Adder teaches that binary math is just logic gates working together. Understanding this circuit prepares us to build more powerful components like Full Adders and multi-bit binary arithmetic units, forming the arithmetic core of computers.

---