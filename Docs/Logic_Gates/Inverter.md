# 🔄 NOT Gate (Inverter)

## 🧠 Overview
Now that we’ve created a NAND gate using relays, we can build a **NOT gate** by connecting **both inputs of a NAND gate to the same signal**.



### 🔁 How It Works
By wiring the same input to both A and B of a NAND gate:

- If the input is `1`, the NAND gate sees `1 & 1 = 1`, then inverts it → **output = 0**
- If the input is `0`, the NAND gate sees `0 & 0 = 0`, then inverts it → **output = 1**

This behavior matches the truth table for a NOT gate and gives us a basic **inverter circuit**.

### 🧰 Why This Matters
With this inverter built from NAND, we now have another essential component to help us construct more complex logic circuits. This simple gate plays a huge role in building ALUs, control logic, and eventually — a full processor.

---

## 🧪 Not Symbol and Truth Table

![not-gate](https://github.com/user-attachments/assets/e005d6c8-d117-407d-a471-31eb02feb77a)
