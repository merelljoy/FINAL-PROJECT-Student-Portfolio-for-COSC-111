# Laboratory Activity #4 Arduino Serial Connection

---
This laboratory activity focuses on implementing **serial communication** in Arduino and using the **Serial Monitor** as a control interface. Building on the circuit and code base from Laboratory Activity #3, the activity demonstrates how sensor data and serial commands can work together to control system behavior.

The system uses **one selected sensor** (thermistor or photoresistor) to trigger an LED alert, which can be manually stopped through a serial command.

---

## Objectives
- Understand and implement Arduino serial communication  
- Familiarize students with basic Serial functions  
- Control an Arduino circuit using Serial input  
- Combine sensor-based logic with user commands via Serial Monitor  

---

## Concepts Applied
- Serial communication using `Serial.begin()`, `Serial.read()`, and `Serial.available()`  
- Case-insensitive string handling  
- Sensor threshold detection  
- State-based control logic  
- Digital output control using Arduino  
- Timing control using `delay()`  

---

## System Overview

### Sensor Selection
The system uses **one sensor**:
- **Thermistor** (temperature threshold: **50°C**), or  
- **Photoresistor** (brightness threshold: **220**)  

### Hardware Configuration
- Selected sensor connected to its respective analog pin  
- **LED connected to digital pin 8**  
- Arduino MCU, resistors, jumper wires, breadboard  

---

## System Behavior
- The Arduino continuously reads the selected sensor value  
- When the sensor reading meets or exceeds the defined threshold:
  - The LED on **pin 8** starts blinking with a **100 ms delay**  
- Once triggered, the LED **continues blinking even if the sensor value goes below the threshold**  
- Entering the word **"stop"** in the Serial Monitor:
  - Stops the LED blinking  
  - Command is **case-insensitive** (e.g., `STOP`, `Stop`, `sToP`)  

---

## Passing Criteria
- Working circuit and Arduino sketch  
- Proper use of Serial communication  
- LED blinking behavior persists after threshold is reached  
- Blinking stops only when `"stop"` is entered via Serial Monitor  

---

## Learning Outcome
This activity helps students understand how **serial communication** can be used to control hardware behavior, enabling interactive and user-controlled IoT systems.
