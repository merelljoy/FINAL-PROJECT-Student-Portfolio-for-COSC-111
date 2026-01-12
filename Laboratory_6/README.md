# Laboratory Activity #6: Bidirectional Control (Arduino & Python)

## Project Overview
This activity demonstrates a two-way connection. When you press a button on the Arduino, it tells Python. Python then sends a command back to the Arduino to turn on an LED. 

---

## Objectives
* Send data from Arduino to Python.
* Send data from Python back to Arduino.
* Maintain a fast response time (under 1 second).

---

## Pin Assignments
### LEDs (Outputs)
* Red: Pin 7
* Green: Pin 6
* Blue: Pin 5

### Buttons (Inputs)
* Button 1: Pin 12 (Sends 'R')
* Button 2: Pin 11 (Sends 'G')
* Button 3: Pin 10 (Sends 'B')

---

## Logic Flow
1. **The Button Press:** You press a button on the breadboard.
2. **Outbound Signal:** Arduino sends a letter ('R', 'G', or 'B') to Python.
3. **Python Processing:** Python receives the letter and immediately sends a number ("1", "2", or "3") back to Arduino.
4. **Inbound Signal:** Arduino receives the number and toggles (ON/OFF) the matching LED.

---

## How to Use
1. **Build:** Connect the LEDs and buttons to the pins listed above.
2. **Upload:** Flash the `.ino` file to your Arduino.
3. **Run:** Start the Python script on your laptop.
4. **Test:** Press a button. The LED should toggle almost instantly.

