# Laboratory Activity #4: Arduino Serial Connection

## Description
This project demonstrates how to control an Arduino using the **Serial Monitor**. It features a "latching" alarm system: once a sensor threshold is triggered, the alarm stays active until a manual "stop" command is sent from the computer.

---

## Objectives
* Use **Serial Communication** to send and receive data.
* Implement **Case-Insensitive** string commands.
* Create a persistent alarm state that requires user intervention to reset.

---

## Hardware Setup
| Component | Pin | Threshold |
| :--- | :--- | :--- |
| **Sensor (User Choice)** | `A0` or `A2` | 50°C (Temp) / 220 (Light) |
| **Alarm LED** | `8` | Blinks at 100ms delay |

---

## Logic & Commands
1. **Trigger:** If the sensor reading exceeds the threshold, the LED on **Pin 8** begins blinking.
2. **Persistence:** The LED continues to blink even if the sensor values return to normal levels.
3. **Reset Command:** To turn off the LED, type `stop` into the Serial Monitor.
   * The command is **case-insensitive** (e.g., `STOP`, `Stop`, and `stop` all work).

---

## 🚀 How to Run
1. Upload the code and open the **Serial Monitor** at **9600 Baud**.
2. Trigger the sensor (apply heat or light).
3. Once the LED starts blinking, type `stop` in the Serial input bar to reset the system.
