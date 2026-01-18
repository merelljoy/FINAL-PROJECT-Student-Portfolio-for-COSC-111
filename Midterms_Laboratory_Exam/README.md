# Midterm Laboratory Examination: Smart Lighting System using Arduino (IoT)

This laboratory activity focuses on designing and programming a smart lighting system using Arduino for an outdoor environment. The system utilizes a photoresistor (LDR) to measure ambient light intensity and automatically controls LED indicators based on predefined thresholds.

The project demonstrates both manual and automatic modes, allowing users to interact with the system through the Serial Monitor to adjust thresholds and switch modes dynamically.

---

## Objectives
- Understand the use of a photoresistor for light intensity sensing  
- Implement threshold-based LED control using Arduino  
- Apply serial communication for user interaction  
- Differentiate between manual and automatic system modes  
- Simulate environmental lighting conditions using sensor data  

---

## Concepts Applied
- Analog sensor data acquisition using `analogRead()`  
- Light intensity conversion from raw values (0–1023) to percentage (0–100%)  
- Threshold-based decision logic  
- Serial communication and command parsing  
- Use of `if-else` and `switch` statements  
- String handling using `startsWith()` and `substring()`  
- Digital output control for LEDs  

---

## System Overview
The system consists of the following components:

- A photoresistor (LDR) connected to an analog pin to measure light intensity  
- Three LEDs representing light levels:
  - Green LED – Low light intensity  
  - Yellow LED – Medium light intensity  
  - Red LED – High light intensity  

Only one LED is active at a time, depending on the detected light level.

The system operates in two modes:

- **Manual Mode** – Users can set custom LOW and HIGH thresholds via the Serial Monitor  
- **Automatic Mode** – Thresholds adjust dynamically to simulate cloudy, normal, and bright sunlight conditions  

Sensor readings, active LED, current mode, and environment status are displayed on the Serial Monitor every second, providing real-time system feedback.
