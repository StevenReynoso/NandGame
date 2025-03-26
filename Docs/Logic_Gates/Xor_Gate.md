# 🔀 XOR Gate (Exclusive OR using NAND Gates)

## 🧠 Overview
The **Exclusive OR gate (XOR)** is a logic gate that outputs `1` only when **one input is HIGH** and the **other is LOW**. If both inputs are the same — either both `0` or both `1` — the output is `0`. This gate behaves differently than the standard OR gate because it **excludes the case where both inputs are HIGH**.

Think back to the OR gate apple analogy: if I give you **one apple**, you have "one or the other" — and that still holds for XOR. But if I give you **both apples**, XOR says "nope" — it's **exclusive**.

---

## 🔢 XOR Truth Table

| A | B | A ⊕ B |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   0    |

---

## ⚖️ Logic Expression
The XOR function can also be represented as:

```plaintext
A XOR B = (A OR B) AND NOT(A AND B)
```

This means that XOR returns true if **either A or B is true**, but **not both**.

---

## ♻️ How to Build XOR Using NANDs
We can construct an XOR gate using **only 4 NAND gates**:

### Step-by-Step NAND Logic:
1. `X = A NAND B`
2. `Y = A NAND X`
3. `Z = B NAND X`
4. `Output = Y NAND Z`

This final output produces the correct XOR behavior.

---

## 📄 What I Learned
- XOR differs from OR by excluding the `1 + 1 = 1` case
- How to build XOR using only **4 NAND gates**
- XOR plays a big role in **adders**, **parity checks**, and other core digital logic systems
- Even though NAND is universal, practical circuits are optimized for **gate count, area, and power**, not just gate type

---

## 🔧 Optimization Insight
While building all gates from NANDs is educational, in real-world hardware design, minimizing gate count is often more important than using only one gate type. XOR is a great example: while it can be built from NANDs, many CPUs and FPGAs use dedicated XOR logic to save space and improve performance.

---

## 📖 Summary
The XOR gate is a fundamental tool in digital logic, and learning how to construct it from NAND gates builds your understanding of logic gate composition, truth tables, and optimization. It also marks a transition point from basic gates to more complex arithmetic and control circuits in your NAND journey.

---

