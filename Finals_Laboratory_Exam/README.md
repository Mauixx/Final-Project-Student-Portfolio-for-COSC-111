# Finals Laboratory Exam: Arduino-to-Python API Client System

## 📜Description

This project involves the design and implementation of an Arduino-to-Python client system where a physical push button connected to an Arduino is used to remotely trigger actions on another Arduino-controlled LED system. The Arduino does not communicate with the API directly; instead, it sends signals to a Python client application via serial communication. The Python client then sends HTTP requests to a predefined API endpoint to control the remote LED system.

## 🖇️Objectives

* Detect valid push button presses using an Arduino
* Implement reliable serial communication between Arduino and Python
* Use Python as an intermediary client for API communication
* Trigger remote LED actions through HTTP requests
* Enforce correct communication and behavior rules between systems

## ⚓Concepts

* Arduino digital input handling and software debouncing
* Serial communication between Arduino and Python
* Client–server architecture
* RESTful API interaction using Python
* Input validation and error handling
* Event-driven system behavior

## ⚙️System Overview

The system is composed of three main parts: an Arduino input device, a Python client application, and a remote API-controlled LED system. The Arduino detects a push button press and sends a single serial signal representing its assigned group number to the Python client. The Python application continuously listens to the serial port, validates and normalizes the received input, and sends an HTTP request to the API endpoint following the required format. Feedback such as the group number, endpoint called, and API response status is displayed in the terminal. Communication rules ensure that each button press results in only one API request and that long presses do not trigger repeated calls.

## 💡Conclusion

This project demonstrates a practical Internet of Things (IoT) architecture where hardware input devices are integrated with web-based services through an intermediary software client. By separating hardware control, serial communication, and API interaction, the system highlights scalable and modular design principles commonly used in real-world IoT applications.


## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `finals_lab_exam.ino` | Arduino code that detects a button press and sends a group number to the computer via serial communication.   |
| `finals_exam_breadboard_diagram.png` | Shows a push button connected to the Arduino using a pull-up configuration for detecting button presses. |
| `finals_lab_exam.py` | Python program that listens to serial data from the Arduino and calls a web API endpoint when a button is pressed. |
