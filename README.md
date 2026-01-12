# Laboratory Activity #2: Working with Analog Signals

## 📌 Project Overview
Building upon the foundations of digital signals, this activity explores **Analog Signals** and **Pulse Width Modulation (PWM)** using Arduino. Instead of simple ON/OFF states, this project implements a running light sequence where LED brightness is controlled via `analogWrite()`, and the code structure is optimized using arrays and loops.

---

## 🎯 Objectives
* **Analog Implementation:** Understand how to simulate analog output on digital pins using PWM.
* **Signal Mapping:** Explore the conversion of values and the logic behind signal modulation.
* **Code Optimization:** Implement `while()` loops and **Arrays** to manage pin modes and LED states efficiently.

---

## 🛠️ Hardware Configuration
The setup uses five LEDs connected to PWM-capable pins (where applicable) or digital pins for signal simulation:
* **LEDs:** Connected to Pins **12, 11, 10, 9, and 8**.
* **Resistors:** 220Ω for each LED.
* **Controller:** Arduino Uno/Mega.



---

## ⚙️ Logic and Instructions
The "Running Light" sequence follows the same directional flow as Activity #1 (Pin 12 to Pin 8) but with updated constraints:

1.  **Array Initialization:** All LED pins are stored in an array, and `pinMode` is set using a `while()` loop to demonstrate efficient code scaling.
2.  **Analog Control:** Instead of `digitalWrite()`, the project uses `analogWrite()` to manage the output signal.
3.  **The Sequence:**
    * **Phase 1:** LEDs turn ON one by one (Pin 12 → 8) with a 1-second delay.
    * **Phase 2:** LEDs turn OFF one by one (Pin 12 → 8) with a 1-second delay.

---

## Repository Contents
* `Activity2_AnalogSignals.ino` — The source code utilizing arrays and while-loops.
* `Circuit_Diagram.png` — Breadboard diagram (TinkerCad/Fritzing).
* `Member_Grades.md` — Document containing group member details and grading breakdown.

---

## How to Run
1.  Clone this repository.
2.  Connect the LEDs to pins 8 through 12 of your Arduino.
3.  Upload the `.ino` sketch via the Arduino IDE.
4.  Observe the sequential lighting effect governed by the array logic.

---
*Submitted as part of the Laboratory requirements for IoT Systems.*
