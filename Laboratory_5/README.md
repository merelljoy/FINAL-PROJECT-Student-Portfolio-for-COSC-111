# Laboratory Activity #5: Arduino-Python Serial Interface

## Description
This project focuses on controlling hardware through a Python script. Using the pyserial library, a computer-based menu is used to toggle LEDs on an Arduino board via Serial communication.

---

## Objectives
* Establish a serial connection between Python and Arduino.
* Implement toggle logic for individual LEDs.
* Create a Command Line Interface (CLI) in Python to send commands.

---

## Hardware Setup
| LED Color | Pin | Command |
| :--- | :--- | :--- |
| Red | 8 | R (Toggle) |
| Green | 9 | G (Toggle) |
| Blue | 10 | B (Toggle) |

---

## Functions and Logic
### Arduino
The Arduino receives serial input and executes the following:
* R, G, B: Toggles the state of the specific LED.
* A: Turns all LEDs on.
* O: Turns all LEDs off.

### Python
The Python script runs a menu loop:
* Clears the screen after each input.
* Handles case-insensitive inputs (e.g., 'r' and 'R' both work).
* X: Closes the connection and exits the program.

