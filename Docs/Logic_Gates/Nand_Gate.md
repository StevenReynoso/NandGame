# 🔌 NAND Gate (Relay-Based)

## 🧠 Overview
This NAND gate is built using two **SPDT (Single Pole Double Throw)** electromechanical relays. The purpose of this circuit is to demonstrate how basic digital logic can be implemented at the hardware level — specifically using mechanical switches instead of modern transistors.

---

## 🧱 The NAND Gate Being Created
The NAND (NOT AND) gate is the inverse of an AND gate, which becomes clear when comparing their truth tables. It's considered the **easiest digital logic gate to implement** using relays and is also the most powerful — since **all other logic gates can be built from NAND gates alone**.

In fact, NAND gates are known as a **"universal gate"** and form the foundation of all digital logic systems. At the lowest level, modern processors use millions (or billions) of logic gates — many of which are based on this exact concept. 


## ⚙️ How It Works

### 🎛️ Relay Basics
Each SPDT relay has:
- A **coil**, which when energized, switches the common contact from the **Normally Closed (NC)** terminal to the **Normally Open (NO)** terminal.
- A **mechanical switch** controlled by the coil.
- Terminals labeled: **COM (common)**, **NC (normally closed)**, and **NO (normally open)**.

### 🔁 Circuit Description
- **Input A** energizes **Relay 1’s coil from a normally closed state to a normally open**
- **Input B** passes voltage through relay one, when input A's relay is on or 1, When input B's input is 1 the relay can pass voltage through the relay now that it is is an normally open state**
- The output is taken from the first relay point to the second relay's coil side, this relay is another SPDT relay but this one is a normally open circuit by default.
- the second input for the second relay is connected directly to voltage, where voltage by default is passed through the circuit since it is a normally open circuit until the coil for the second relay is energized.

When **both inputs (A and B)** are HIGH (energizing both coils), causing the second relay to switch away from the NO contact, breaking the path to the output. This causes the output to be pulled LOW.  
In **all other input combinations**, at least one relay remains unenergized, keeping the voltage to be passed through the second relay in its NO default state — allowing voltage to reach the output. This satisfies the NAND logic truth table.

---

## 🧪 NAND Symbol and Truth Table

![nand-gate](https://github.com/user-attachments/assets/f4a57c98-4fa1-4608-8b8b-6432075807cc)

---

## 📝 What I Learned

- How **relays can physically represent logic gates** by controlling current flow.
- Why **NAND gates are universal**, meaning all logic can be built from them.
- The difference between **normally open vs. normally closed contacts**.
- How **modern logic gates use transistors**, which are faster, consume less power, and don’t suffer from contact bounce like mechanical relays.
- Real-world implications of switching speed and durability in digital systems.

---

## 🔍 Notes

Relays are rarely used in digital computing today due to:
- **Slower switching speeds**
- **Mechanical wear**
- **Size and power consumption**

However, understanding relay-based logic is a fantastic way to learn the fundamentals of **digital logic and hardware abstraction** from the ground up.

