# Midterms Laboratory Exam: Smart Lighting System Using Arduino

##  📜Description

 This project involves designing and programming a smart lighting system using an Arduino for an outdoor environment. The system uses a photoresistor to measure ambient light intensity and controls three LEDs to visually represent lighting conditions. It supports both manual and automatic modes, allowing users to either define custom light thresholds or let the system adjust automatically based on environmental conditions such as cloudy or bright sunlight. 

## 🖇️Objectives 

* Measure ambient light intensity using a photoresistor
* Convert analog sensor readings into percentage-based light intensity values
* Control LEDs to represent different light levels
* Implement manual and automatic operating modes
* Enable user interaction through the serial monitor

## ⚓Concepts 

* Analog-to-digital conversion using Arduino
* Sensor-based input processing (photoresistor)
* Conditional logic and threshold-based decision making
* Serial communication for user interaction
* State-based system design (Manual vs Automatic modes)

## ⚙️System Overview

The system uses a photoresistor connected to an analog pin to continuously read light intensity values. These readings are mapped from 0–1023 to 0–100%. Based on predefined thresholds, only one LED is activated at a time to indicate low, medium, or high light intensity. In manual mode, users can switch modes and configure threshold values using serial commands. In automatic mode, the system dynamically adjusts threshold values to simulate different environmental lighting conditions such as cloudy, normal, or bright sunlight. System status, including light intensity, active LED, current mode, and environment state, is displayed on the serial monitor every second.

## 💡Conclusion

This project demonstrates the practical application of Arduino in building an intelligent lighting system that responds to environmental changes. By integrating sensors, LEDs, and serial communication, the system highlights key concepts in embedded systems, automation, and user-controlled hardware behavior.


## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `midterms_lab_exam.ino` | Arduino program that reads light intensity from a photoresistor and controls LEDs in manual or automatic mode using serial commands. |
| `midterms_lab_exam_breadboard_diagram.png` | Illustrates how the Arduino connects to the photoresistor and the green, yellow, and red LEDs for light-based control. |
