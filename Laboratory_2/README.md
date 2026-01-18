# Laboratory Activity #2 Working with Analog Signals

---

## Description
This laboratory activity introduces **analog signals** and their implementation in an Arduino circuit. Building on the concepts from the first activity, this exercise enhances the running light system by controlling the **brightness of LEDs** using analog signals.

The activity also demonstrates **analog-to-digital signal conversion** and the use of the `map()` function to convert sensor or value ranges into appropriate output levels.

---

## Objectives
- Understand analog signals and their role in Arduino circuits  
- Learn how analog values are represented digitally in Arduino  
- Apply the `map()` function for analog-to-digital signal conversion  
- Control LED brightness using `analogWrite()`  
- Utilize arrays and `while()` loops for efficient pin management  

---

## Concepts Applied
- Analog vs digital signals  
- Pulse Width Modulation (PWM)  
- LED brightness control using `analogWrite()`  
- Analog-to-digital value mapping using `map()`  
- Use of arrays for pin configuration  
- Looping structures using `while()`  

---

## System Overview
The system consists of a **running light circuit** with brightness-controlled LEDs.

### Hardware Configuration
- Arduino MCU  
- Five LEDs connected to digital pins **8 to 12**  
- Resistors, jumper wires, and breadboard  

### Circuit Behavior
- LEDs turn ON sequentially from **pin 12 down to pin 8**  
- LED brightness is controlled using `analogWrite()`  
- Each LED transition has a **1-second delay**  
- After all LEDs turn ON, they turn OFF one by one in the same order  
- Pin modes are set using an **array** and controlled using a **while() loop**  

---

## Expected Output
- LEDs brighten sequentially from pin 12 to pin 8  
- LEDs dim or turn off sequentially from pin 12 to pin 8  
- The running light effect continuously repeats with analog brightness control  

---

## Learning Outcome
This activity helps students understand how **analog signals** and **PWM** are used in Arduino to control output intensity, forming a foundation for sensor-based and adaptive IoT applications.
