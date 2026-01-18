# Laboratory Activity #1 Working with Digital Signals

---

This laboratory activity introduces the fundamentals of **digital signals** using Arduino as a core device for **IoT systems implementation**. The activity focuses on controlling digital outputs by creating a **running light circuit**, where multiple LEDs are turned on and off in a specific sequence.

Through this exercise, students gain hands-on experience with digital signal control using Arduino’s GPIO pins.

---

## Objectives
- Review Arduino as a platform for IoT system implementation  
- Understand digital signals and their behavior in an Arduino circuit  
- Learn how to control digital outputs using `digitalWrite()`  
- Implement timing control using delay functions  

---

## Concepts Applied
- Digital input and output signals  
- GPIO pin configuration using `pinMode()`  
- LED control using `digitalWrite()`  
- Looping structures for sequential execution  
- Timing control using `delay()`  

---

## System Overview
The system consists of a **running light circuit** using five LEDs connected to the Arduino.

### Hardware Configuration
- Arduino MCU  
- Five LEDs connected to digital pins **8 to 12**  
- Resistors and jumper wires  
- Breadboard  

### Circuit Behavior
- LEDs turn **ON one by one** starting from **pin 12 down to pin 8**  
- After all LEDs are ON, they turn **OFF one by one** in the same order  
- Each LED change has a **1-second delay**  
- LED states are controlled using the `digitalWrite()` function  

---

## Expected Output
- LEDs light up sequentially from pin 12 to pin 8  
- LEDs turn off sequentially from pin 12 to pin 8  
- The running light pattern continuously repeats  

---

## Learning Outcome
This activity strengthens understanding of **digital signal control** in Arduino and builds a foundation for more advanced IoT and automation projects.
