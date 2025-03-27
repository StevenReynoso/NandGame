# ➕ Full Adder (3-Input Binary Adder)

## 🧠 Overview
The **Full Adder** is a digital circuit that adds **three 1-bit binary inputs**:
- Two primary inputs: `A` and `B`
- One **carry-in** input: `Cin`

It produces two outputs:
- **Sum**: The result of the binary addition
- **Carry-out**: Overflow bit to be carried to the next higher bit position

Unlike the **Half Adder**, which could only add two inputs, the Full Adder allows you to **chain multiple adders together**, enabling multi-bit binary addition — like 4-bit or 8-bit adders used in real processors.

---

## 🔢 Truth Table

![adder-table](https://github.com/user-attachments/assets/8d6eb4e4-d294-40e4-a918-0cfa9c799f9d)


---

## ⚙️ How It Works
A Full Adder can be constructed using **two Half Adders and an OR gate**:

1. First Half Adder: `A + B` → produces intermediate **Sum1** and **Carry1**
2. Second Half Adder: `Sum1 + Cin` → final **Sum** and **Carry2**
3. OR Gate: combines `Carry1` and `Carry2` → produces final **Carry-out**

This modular approach shows how we can build increasingly complex logic by **stacking simpler blocks**.

---

## ⚖️ Logic Expressions
- **Sum = A XOR B XOR Cin**
- **Cout = (A AND B) OR (Cin AND (A XOR B))**

---

## ♻️ Gate Implementation Using NANDs
To build a Full Adder using only NAND gates:
![0b78609b-fe0d-42f2-a715-bdc4584a07f83868143203346644687](https://github.com/user-attachments/assets/37aa4de8-8829-4fc4-9f4a-4cbe5a3009f0)

while this may be some what confusing on how to eliminate some nand gates, you would need 9 nand gates, instead of using the 3 components we used in our full adder level

Total: **9 Nand Gates** minimum

---

## 📄 What I Learned
- The Full Adder introduces **carry-in logic**, enabling multi-bit binary addition
- Two Half Adders + OR = Full Adder — circuits build on top of one another
- Logic expressions for full addition can be broken into reusable subcomponents
- Real CPUs use these principles at the hardware level for all addition operations

---

## 🔧 Why It Matters
The Full Adder is the foundation of all binary arithmetic in digital systems. Whether it’s adding two numbers in your calculator or executing an instruction in a CPU — it all starts here. Understanding Full Adders helps bridge logic design with arithmetic circuits that power every digital system.

---

