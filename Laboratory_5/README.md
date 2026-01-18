# Laboratory Activity #5: Receiving Serial Connection Using Arduino from Python

---
This laboratory activity demonstrates how Arduino can **receive and process serial commands from a Python application**. The system establishes a serial connection between Arduino and Python using the `pyserial` library, enabling external software to control hardware components in real time.

The activity highlights **bi-directional interaction**, **case-insensitive command handling**, and **menu-driven control** using Python.

---

## Objectives
- Understand and implement Arduino serial communication  
- Utilize Python as a tool for serial connection using `pyserial`  
- Control Arduino hardware through external software  
- Apply case-insensitive command processing  

---

## Concepts Applied
- Serial communication between Arduino and Python  
- Character-based command parsing  
- Case-insensitive input handling  
- Digital output control for LEDs  
- Menu-driven console applications in Python  
- Program flow control and loop termination  

---

## System Overview

### Hardware Components
- Arduino MCU  
- Three LEDs:
  - Red LED → Pin 8  
  - Green LED → Pin 9  
  - Blue LED → Pin 10  
- Resistors, jumper wires, breadboard  

### Software Components
- Arduino IDE  
- Python  
- PySerial library  

---

## System Behavior

### Arduino (Serial Input Handling)
The Arduino listens for serial input and performs the following actions:

- `R` / `r` → Toggle **Red LED**  
- `G` / `g` → Toggle **Green LED**  
- `B` / `b` → Toggle **Blue LED**  
- `A` / `a` → Turn **all LEDs ON**  
- `O` / `o` → Turn **all LEDs OFF**  
- Any other input → Returns an **error message**

All inputs are **case-insensitive**.

---

### Python Application Behavior
The Python script runs in a **non-terminating loop** and displays the following menu:
[R] Red ON/OFF
[G] Green ON/OFF
[B] Blue ON/OFF
[A] All ON
[O] All OFF
[X] Exit

- User input is sent to Arduino via serial connection  
- Input `X` / `x` terminates the Python application  
- All inputs are **case-insensitive**

---

## Nice-to-Have Features
- Clear the console screen after every input and reprint the menu  
- Organize common Arduino functions inside a header file  

---

## Expected Output
- LEDs respond correctly to serial commands from Python  
- Invalid inputs return error messages from Arduino  
- Python application exits cleanly when `X` is entered  

---

## Learning Outcome
This activity strengthens understanding of **cross-platform serial communication**, demonstrating how **Python applications can control Arduino hardware**, a core concept in IoT and automation systems.


