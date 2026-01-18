# Final Laboratory Examination Arduino-to-Python Client System (IoT)

---

This laboratory activity focuses on designing and implementing an **Arduino-to-Python client system** that enables remote control of an LED system through a **Python-based API client**. Instead of directly communicating with an API, the Arduino sends signals via **Serial communication** to a Python program, which then triggers predefined API endpoints.

The activity emphasizes **decoupling hardware from web services**, proper input validation, and controlled communication behavior.

---
## Objectives
- Implement Arduino serial communication using push buttons  
- Develop a Python client that listens to serial input continuously  
- Trigger HTTP API requests based on Arduino signals  
- Enforce proper communication and debouncing rules  
- Demonstrate real-world IoT client–server interaction  

---
## Concepts Applied
- Serial communication between Arduino and Python  
- Software debouncing for button inputs  
- Non-terminating Python applications  
- REST API request handling  
- Input validation and normalization  
- Separation of concerns in IoT systems  
---
## System Overview
### Arduino Responsibilities
- Uses a **push button** as the input device  
- Detects valid button presses with **software debouncing**  
- Sends **only one signal per press** via Serial Monitor  
- Sends a signal representing the **assigned group number**  
- Does **not**:
  - Make HTTP requests  
  - Control LEDs directly  
---
### Python Client Responsibilities
- Continuously listens to the serial port (non-terminating)  
- Receives and validates input from Arduino  
- Extracts and normalizes the **group number**  
- Sends an HTTP request to the API using the format:

