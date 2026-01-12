# Laboratory Activity #1: Working with Digital Signals

## Project Overview
This project is the first laboratory activity for the **IoT Systems Implementation** course. It focuses on the fundamental application of **Digital Signals** using the Arduino platform. The goal is to create a "Running Light" circuit that demonstrates sequential control of hardware outputs.

---

## Objectives
* **Review Arduino:** Re-evaluate Arduino’s role as a primary controller in IoT system implementation.
* **Signal Implementation:** Apply digital signals (HIGH/LOW) within an Arduino circuit using the `digitalWrite()` function.

---

## 🛠️ Hardware Configuration
The circuit consists of five LEDs connected to the following Arduino Digital Pins:
* **LED 1:** Pin 12
* **LED 2:** Pin 11
* **LED 3:** Pin 10
* **LED 4:** Pin 9
* **LED 5:** Pin 8

---

## Logic and Instructions
The program follows a specific sequence with a **1-second (1000ms) delay** between each state change:

1.  **Sequential Power-Up:** Turn all LEDs **ON** one by one, starting from **Pin 12** down to **Pin 8**.
2.  **Sequential Power-Down:** Turn all LEDs **OFF** one by one, starting from **Pin 12** down to **Pin 8**.

delay(1000);
digitalWrite(11, HIGH);
// ... and so on
