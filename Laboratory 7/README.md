# Laboratory Activity #7: Controlling Arduino using FastAPI

---
## 📖Description

This laboratory activity focuses on controlling an Arduino microcontroller through a web-based interface using FastAPI. The system uses serial communication to enable interaction between hardware components (LEDs and buttons) and a Python application. By sending HTTP requests, users can control LEDs connected to the Arduino in real time.

---
## 🎯Objectives

* Understand how Arduino communicates with external applications using serial communication
* Apply Python as a tool for controlling hardware devices
* Implement a simple HTTP-based control system using FastAPI
* Demonstrate bi-directional communication between Arduino and a Python web server

---
## 💡Concepts Applied

* Arduino digital input and output control
* Serial communication between Arduino and Python
* Python programming using pyserial
* RESTful API development using FastAPI
* Hardware–software integration

---
## 🛠️System Overview

The system consists of an Arduino connected to three LEDs and three push buttons. The Arduino listens for serial commands sent by a FastAPI server running in Python. Each HTTP request triggers the Python application to send a specific character through the serial port, which the Arduino interprets to toggle or control the LEDs. This setup allows LED control via a web browser or API client.

---
## ⭐Conclusion

This laboratory activity demonstrates how embedded systems can be integrated with web technologies. By combining Arduino, Python, and FastAPI, the project shows an effective method of controlling physical hardware through HTTP requests, reinforcing concepts in serial communication, API development, and system integration.

---

## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `lab7_activity.ino` | Arduino code that reads button presses and serial commands to toggle the red, green, and blue LEDs.  |
| `lab7_breadboard_diagram.png` | Shows how the Arduino, buttons, LEDs, resistors, and wires are physically connected. |
| `lab7_activity.py` | Python FastAPI program that sends serial commands to the Arduino to control the LEDs through a web API. |
