# Laboratory Activity #3: Working with Sensors

## 📜Description

This activity introduces the use of sensors in Arduino circuits for IoT applications. Students will create a simple fire detection system using a **thermistor** to measure temperature and a **photoresistor** to detect brightness. When temperature or brightness exceeds defined thresholds, the system signals a fire using a fast-blinking LED and optionally a buzzer.



## 🖇️Objectives

* Familiarize students with basic sensor components for IoT
* Integrate sensors into an Arduino circuit
* Implement a simple fire sensor system



## ⚓Concepts

* Analog sensor reading with **thermistors** and **photoresistors**
* Threshold-based detection and alerts
* Use of functions to separate sensor readings
* Pin management using `#define`
* Threshold management using `const`
* Digital output for notification (LED and optional buzzer)


## ⚙️System Overview

The system uses:

* **A0** for the thermistor (temperature sensor)
* **A2** for the photoresistor (brightness sensor)
* **Pin 12** for a red LED (fire alert)
* Optional buzzer on the same pin as the LED

The Arduino continuously reads temperature and brightness. If the temperature exceeds **50°C** or the brightness exceeds **220**, the LED blinks rapidly to indicate a fire. The readings for temperature and brightness are handled in separate functions, and pin numbers and threshold values are defined for easier code management.

## 💡Conclusion

This activity demonstrates the practical use of sensors in detecting real-world conditions and responding through appropriate alerts. By combining temperature and light sensing with threshold logic, students gain hands-on experience in building a simple but effective fire detection system. The project reinforces key IoT concepts such as sensor integration, modular programming, and real-time system response.


## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `lab3_activity.ino` | Arduino sketch for thermistor and photoresistor sensing with fire alert logic |
| `lab3_breadboard_diagram.png` | Breadboard diagram showing sensor and alert component connections |

