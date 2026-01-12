# Laboratory Activity #6: Bidirectional Control Using Arduino and Python

## 📖 Description

This activity introduces **bidirectional serial communication** between Arduino and Python. Students will build a circuit with three LEDs and three push buttons. Arduino will send signals to Python when buttons are pressed, and Python will respond by sending commands back to toggle specific LEDs. This demonstrates interactive control and real-time feedback in Arduino-Python systems.

---

## 🎯 Objectives

* Understand and implement Arduino Serial communication
* Use Python to interact with Arduino in real time
* Create a bidirectional control system where Arduino sends signals to Python and receives commands back

---

## 💡 Concepts Applied

* Serial communication for two-way data exchange
* Button input detection in Arduino
* LED control based on Python commands
* Case-insensitive command handling
* Real-time response (<1 second)
* Modular programming using functions for button and LED management

---

## 🛠 System Overview

* **Components:** Arduino MCU, 3 LEDs (Red, Green, Blue), 3 push buttons, resistors, wires, breadboard, laptop with Python and `pyserial`

* **Pin Assignment:**

  * LEDs → Red: 7, Green: 6, Blue: 5
  * Buttons → Button1: 12, Button2: 11, Button3: 10

* **Arduino Sketch Behavior:**

  * **Outbound:** Pressing a button sends a single character (`R`, `G`, `B`) to Python; no LED action occurs
  * **Inbound:** Arduino toggles LEDs when receiving `1`, `2`, or `3` from Python

* **Python Script Behavior:**

  * Receives button signals from Arduino (`R`, `G`, `B`)
  * Sends back `1`, `2`, or `3` to Arduino to toggle the corresponding LED
  * Runs continuously and responds within <1 second

---

## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `lab6_activity.ino` |Arduino sketch managing button input, sending signals to Python, and toggling LEDs based on Python commands|
| `lab6_activity.py` | Python script receiving signals from Arduino buttons and sending back commands to control LEDs |
| `lab6_breadboard_diagram.png` | Breadboard diagram showing connections for buttons, LEDs, and Arduino pins |
