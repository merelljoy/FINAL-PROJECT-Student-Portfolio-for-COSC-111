# Laboratory Activity #3 Working with Sensors

---
This laboratory activity introduces the use of **sensor components** commonly applied in IoT systems and demonstrates how multiple sensors can be integrated into a single Arduino-based circuit. The activity implements a **simple fire detection system** using a **thermistor** and a **photoresistor**.

By combining temperature and light intensity readings, the system illustrates how environmental data can be processed to trigger hardware-based alerts.

---

## Objectives
- Familiarize students with basic sensor components used in IoT  
- Integrate multiple sensors into an Arduino circuit  
- Implement a simple fire detection mechanism using sensor data  

---

## Concepts Applied
- Analog sensor data acquisition  
- Thermistor temperature calculation in Celsius  
- Light intensity sensing using a photoresistor  
- Threshold-based decision logic  
- Function modularization for sensor readings  
- Use of `#define` for pin configuration  
- Use of `const` for fixed threshold values  
- Digital output control for alert signaling  

---

## System Overview
The system uses two sensors to detect potential fire conditions:

### Sensor Configuration
- **Thermistor** connected to analog pin **A0** for temperature measurement (Celsius)  
- **Photoresistor** connected to analog pin **A2** for brightness detection  

### Alert Mechanism
- **Red LED** connected to digital pin **12**  
- *(Optional)* Buzzer or speaker connected to the same pin  

---

## System Behavior
- Temperature and brightness readings are handled in **separate functions**  
- Threshold limits:
  - Temperature ≥ **50°C**  
  - Brightness ≥ **220**  
- When **both thresholds are exceeded**, the system triggers a **fast blinking red LED**  
- The LED (and optional buzzer) serves as a visual and audible fire alert  

---

## Passing Criteria
- Working Arduino circuit and sketch  
- Separate functions for temperature and brightness readings  
- Use of `#define` for pin assignments  
- Use of `const` variables for threshold values  

---

## Learning Outcome
This activity strengthens understanding of **sensor integration**, **environmental data processing**, and **alert-based decision logic**, which are essential concepts in IoT and safety-related systems.
