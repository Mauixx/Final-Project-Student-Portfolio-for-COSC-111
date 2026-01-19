# Laboratory Activity #4: Arduino Serial Connection

##  📜Description

This activity introduces **Arduino Serial communication** to control circuits interactively. Using one sensor from the previous activity (thermistor or photoresistor), students implement a system where an LED blinks when a threshold is exceeded and can be stopped via Serial commands entered from the Arduino Serial Monitor. This reinforces sensor monitoring and basic Serial interaction in Arduino-based IoT systems.


## 🖇️Objectives

* Understand and implement Arduino Serial communication
* Familiarize with basic Serial functions (`Serial.begin()`, `Serial.readString()`, etc.)
* Create a circuit controllable through Serial input


## ⚓Concepts 

* Serial communication for input/output control
* Threshold-based sensor monitoring
* Persistent LED blinking independent of sensor state
* Case-insensitive string handling in Serial input
* Pin and threshold management using `#define` and `const`
* Code modularity using functions


## ⚙️System Overview

* Uses **one sensor** from Activity #3:

  * Thermistor (temperature) → threshold: **50°C**
  * Photoresistor (brightness) → threshold: **220**
* **Pin 8** is assigned to the blinking LED
* LED blinks continuously if threshold is met, even when sensor reading drops below the threshold
* Users can stop the LED by typing **"stop"** (case insensitive) in the Serial Monitor
* Serial communication handles user input and controls the circuit accordingly

## 💡Conclusion

This laboratory activity demonstrates how Serial communication can be used to interactively control Arduino-based systems. By integrating sensor monitoring with Serial input, students learn how hardware behavior can be modified in real time through user commands. The activity reinforces essential IoT concepts such as event-driven control, sensor-based decision making, and reliable communication between users and embedded systems.
---
## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `lab4_activity.ino` | Arduino sketch for sensor-based LED control with Serial input to start/stop blinking|
| `lab4_breadboard_diagram.png` |Breadboard diagram showing Arduino, sensor, LED, and resistor connections |

