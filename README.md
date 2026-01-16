# Laboratory Activity #7: Controlling Arduino using FastAPI

## Description
This project demonstrates how to control an Arduino board via a web-based API. By using **FastAPI**, we can send HTTP requests (URLs) to a Python server, which then communicates with the Arduino through a Serial connection to toggle LEDs.

---

## Objectives
* Connect an Arduino to a Python web server.
* Use **FastAPI** to create web endpoints for hardware control.
* Implement bi-directional logic between a web interface and physical circuits.

---

## Hardware Setup
The following pins are used for the circuit:

| LED Color | Arduino Pin | Serial Command |
| :--- | :--- | :--- |
| Red | 7 | "1" |
| Green | 6 | "2" |
| Blue | 5 | "3" |



---

## API Endpoints
Once the FastAPI server is running, you can control the LEDs using these URL paths:

* **Individual Control:**
  * `/led/red` - Toggles the Red LED
  * `/led/green` - Toggles the Green LED
  * `/led/blue` - Toggles the Blue LED
* **Group Control:**
  * `/led/on` - Turns all LEDs ON
  * `/led/off` - Turns all LEDs OFF

---

## How it Works
1. **Arduino:** Listens for serial inputs ("1", "2", or "3") and toggles the corresponding LED.
2. **FastAPI:** Acts as a bridge. When you visit a specific URL, Python sends the correct command to the Arduino via the Serial port.
3. **Execution:** The LED state changes instantly based on the web request.


