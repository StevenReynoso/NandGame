# ➕ Half Adder (1-Bit Binary Adder)

## 🧠 Overview
The **Half Adder** is a fundamental digital circuit that adds **two 1-bit binary numbers** — inputs `A` and `B`. It produces two outputs:

- **Sum**: The result of the addition
- **Carry**: A bit that represents overflow when both inputs are 1
- ## NandGame makes these as 'h' and 'I' ##

The Half Adder is called "half" because it does **not handle a carry-in** from a previous addition — for that, we'll need a **Full Adder**. This circuit is a building block for more complex arithmetic units like multi-bit adders and ALUs.

---

## 🔢 1-bit Binary Additions
![possibleSums-2-768x212](https://github.com/user-attachments/assets/4ffdacfb-c4c8-4512-bbae-ed54957db62f)

These are the possible sums for the half adder, they are very simple addition, the highest possible number is 10 in binary, which is just 2. You can see where we might need to do a lot more for just adding bigger numbers.


## 🔢 Truth Table and Symbols

![image](https://github.com/user-attachments/assets/5f500a83-c431-4a5c-87ca-42e9c73129eb)

In our truth table you can see the output S and output C might look a bit familiar truth tables from before. Output S is in fact the same XOR truth table as before, and this might lead you to see, we need this for our circuit, Output C also we have seen before, this being the same truth logic for an AND gate. Showing our circuit now to build our half adder we can use an XOR and a AND gate, just 2 gates to make the start of something powerful.

![halfadder2-1-768x320](https://github.com/user-attachments/assets/097cbad5-d9ae-4eff-9783-1745b75c5ca5)

This is the circuit diagram on how to make the half adder, we can see the XOR and the AND gate being used, going to a sum and a Carry output. 

![half-adder-boxitem](https://github.com/user-attachments/assets/1ab1dd83-8b81-4009-b91d-2d4cc5caa20d)

This is something your likely to see instead of when showing a adder on a circuit, a box that says adder with just the inputs and outputs being shown.


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
