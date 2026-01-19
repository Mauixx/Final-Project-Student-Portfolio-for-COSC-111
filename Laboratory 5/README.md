# Laboratory Activity #5: Receiving Serial Connection Using Arduino from Python

##  📜Description

This activity demonstrates **Arduino-Python serial communication** for controlling hardware. Students will build a circuit with three LEDs and write an Arduino sketch to respond to serial commands. A Python script will send commands to toggle individual LEDs, turn all LEDs on or off, or exit the program, allowing interactive control from a computer.


## 🖇️Objectives

* Understand and implement Arduino Serial communication
* Use Python to send commands to Arduino over Serial
* Create a circuit controllable via Serial commands from Python


## ⚓Concepts 

* Serial communication between Arduino and a computer
* Case-insensitive command handling
* LED control via Arduino based on serial input
* Python integration using `pyserial`
* Non-terminating Python loops for interactive control
* Error handling for invalid inputs


## ⚙️System Overview

* **Components:** Arduino MCU, 3 LEDs (Red, Green, Blue), resistors, wires, breadboard, and a laptop with Python and `pyserial` installed
* **LED Pin Assignment:** Red → 8, Green → 9, Blue → 10
* **Arduino Sketch:**

  * Responds to serial input to toggle LEDs:

    * `R/r` → Red LED ON/OFF
    * `G/g` → Green LED ON/OFF
    * `B/b` → Blue LED ON/OFF
    * `A/a` → All LEDs ON
    * `O/o` → All LEDs OFF
    * Any other input → Error message
* **Python Script:**

  * Provides an interactive menu for sending serial commands
  * Commands mirror Arduino logic
  * `X/x` exits the Python application
  * Input is case-insensitive

## 💡Conclusion

This laboratory activity highlights the integration of Arduino and Python through serial communication, demonstrating how software applications can directly control hardware devices. By combining embedded programming with Python-based interaction, students gain practical experience in building interactive IoT-style systems, reinforcing concepts such as serial protocols, modular code design, and cross-platform communication.


## 🗂 Files Included
| File Name | Description |
|-----------|-------------|
| `lab5_activity.ino` | Arduino sketch for receiving serial commands and controlling the red, green, and blue LEDs accordingly |
| `lab5_activity.py` | Python script providing an interactive menu to send serial commands to the Arduino |
| `lab5_activity_functions.h` | Header file with reusable functions for LED control (toggleRed, toggleGreen, toggleBlue, allOn, allOff) |
| `lab5_breadboard_diagram.png` | Breadboard diagram showing the connection of LEDs to Arduino pins 8, 9, and 10|
