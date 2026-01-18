# Laboratory Activity #6 Bidirectional Control Using Arduino and Python

---
This laboratory activity demonstrates **bi-directional serial communication** between Arduino and Python. The system allows Arduino to **send signals to Python** using push buttons (outbound communication) and enables Python to **send control commands back to Arduino** to toggle LEDs (inbound communication).

This activity highlights real-time interaction between hardware inputs and software responses, a key concept in IoT systems.

---

## Objectives
- Understand and implement Arduino serial communication  
- Utilize Python as a tool for serial communication using `pyserial`  
- Create a bi-directional communication system between Arduino and Python  
- Achieve responsive hardware–software interaction  

---

## Concepts Applied
- Bi-directional serial communication  
- Event-based button input handling  
- Case-insensitive serial command processing  
- Digital output control for LEDs  
- Non-terminating Python scripts  
- Low-latency system response design  

---

## System Overview

### Hardware Components
- Arduino MCU  
- Three LEDs:
  - Red LED → Pin 7  
  - Green LED → Pin 6  
  - Blue LED → Pin 5  
- Three Push Buttons:
  - Button 1 → Pin 12  
  - Button 2 → Pin 11  
  - Button 3 → Pin 10  
- Resistors, jumper wires, breadboard  

### Software Components
- Arduino IDE  
- Python  
- PySerial library  

---
## System Behavior

### 📤 Arduino → Python (Outbound Signal)
- Button 1 → Sends `'R'` **once per press**  
- Button 2 → Sends `'G'` **once per press**  
- Button 3 → Sends `'B'` **once per press**  
- Button presses **only send serial data**  
- **No LED actions** occur on Arduino during outbound signaling  

---

### Python → Arduino (Inbound Signal)
- Receives `'R'` → Sends `"1"` back to Arduino  
- Receives `'G'` → Sends `"2"` back to Arduino  
- Receives `'B'` → Sends `"3"` back to Arduino  

Arduino reacts as follows:
- `"1"` → Toggles **Red LED**  
- `"2"` → Toggles **Green LED**  
- `"3"` → Toggles **Blue LED**  

All serial inputs are **case-insensitive**.

---
## Performance Requirement
- System response time must be **less than 1 second** from button press to LED action  

---

## Expected Output
- Button presses on Arduino are detected by Python  
- Python sends corresponding commands back to Arduino  
- LEDs toggle correctly based on returned commands  
- Communication occurs with minimal delay  

---

## Learning Outcome
This activity strengthens understanding of **real-time bi-directional communication** between hardware and software, preparing students for more advanced IoT and automation applications.
