# Laboratory Activity #7  
## Controlling Arduino Using FastAPI

---

This laboratory activity demonstrates how to control an Arduino-based circuit using a **Python backend powered by FastAPI**. The system establishes a **bi-directional serial communication** between Arduino and Python, allowing LEDs to be controlled either through **API endpoints** or **serial input**.

By integrating Arduino hardware with an HTTP-based API, this activity showcases a basic Internet of Things (IoT) concept where physical devices can be controlled through web technologies.

---

## Objectives
- Understand and implement Arduino serial communication  
- Utilize Python as a tool for serial communication using `pyserial`  
- Implement an HTTP-based control system using FastAPI  
- Create a simple bi-directional communication between Arduino and Python  

---

## Concepts Applied
- Serial communication between Arduino and Python  
- HTTP request handling using FastAPI  
- RESTful API design  
- Case-insensitive command processing  
- Digital output control using Arduino  
- Hardware–software integration for IoT applications  

---

## System Overview
The system is composed of the following components:

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
- Breadboard, resistors, jumper wires  

### Software Components
- Arduino IDE  
- Python  
- FastAPI  
- PySerial  

---

## System Behavior

### Arduino (Inbound Serial Commands)
- Input `"1"` → Toggles **Red LED**  
- Input `"2"` → Toggles **Green LED**  
- Input `"3"` → Toggles **Blue LED**  
- All inputs are **case-insensitive**

---

## FastAPI Endpoints

### `/led/{color}`
- `color` can be `red`, `green`, or `blue`
- Sends the following serial commands to Arduino:
  - `red` → `"1"`
  - `green` → `"2"`
  - `blue` → `"3"`

### `/led/on`
- Turns **all LEDs ON**

### `/led/off`
- Turns **all LEDs OFF**

---

## Expected Output
- LEDs respond to API requests sent through FastAPI  
- Arduino receives serial commands from Python and updates LED states accordingly  
- Demonstrates real-time interaction between web services and physical hardware  

---

## Learning Outcome
This activity helps students understand how **web technologies**, **Python**, and **microcontrollers** can work together to form a basic IoT system capable of remote hardware control.
