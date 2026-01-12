# Laboratory Activity #3: Fire Sensor Simulation

## Description
This project simulates a fire alarm system using an Arduino. It monitors two inputs: **Temperature** (via a Thermistor) and **Light** (via a Photoresistor). If both the heat and the brightness reach a specific limit, the system triggers a flashing alarm.

---

## Objectives
* Use sensors to gather environmental data.
* Convert analog signals into meaningful units (Celsius).
* Create a safety logic gate (IF Temperature AND Light are high, THEN alarm).

---

## Hardware Setup
| Component | Pin | Purpose |
| :--- | :--- | :--- |
| **Thermistor** | `A0` | Measures heat |
| **Photoresistor** | `A2` | Measures brightness |
| **Red LED & Buzzer**| `12` | Visual and audio alarm |

---

## How it Works
The system follows these safety rules:
1. **Temperature Threshold:** > 50°C
2. **Brightness Threshold:** > 220
3. **Action:** If **both** are met, the LED and Buzzer on Pin 12 blink/beep rapidly.

### Code Features
* **Functions:** Separate functions for reading temperature and light.
* **Definitions:** Uses `#define` for pins and `const` for thresholds to keep the code organized and easy to change.


