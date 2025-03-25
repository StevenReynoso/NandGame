# 🤝 AND Gate (Built Using NAND + NOT)

## 🧠 Overview
An **AND gate** takes two inputs and returns HIGH (`1`) only if **both inputs are HIGH** at the same time. In logical terms, this is `A AND B`.

The output of the AND gate is the **exact inverse** of a NAND gate’s output. So, if we already have a NAND gate, we can build an AND gate by simply **inverting the output** of the NAND.

---

## 🔁 How It Works

1. Inputs `A` and `B` are fed into a **NAND gate**.
2. The **output of the NAND gate** is then passed through a **NOT gate** (inverter).
3. The result is equivalent to `NOT(NAND(A, B))` → which is exactly `AND(A, B)`.

This construction shows how we can build more complex logic by **chaining simple gates**, starting from just NAND.

---

## 🧪 Symbol and Truth Table

![and-gate](https://github.com/user-attachments/assets/20adade7-9668-49ef-9318-f97ff1a451e1)


You might notice this looks almost identical to a NAND gate. The only visual difference is the **missing circle** (inversion bubble) at the tip of the NAND gate symbol. That small circle represents the **inversion** — so when it’s not there, we’re just looking at an AND gate.

It might be confusing at first, but the symbol differences become second nature with practice.

---

## 📝 What I Learned

- How to build an **AND gate using NAND and NOT gates**
- That **inverters are powerful**, allowing us to transform gates into their opposite
- The significance of logic gate symbols and how **small visual cues** (like the inverter circle) carry meaning
- How simple gates **combine into more complex logic**, which is how real processors are designed

---

