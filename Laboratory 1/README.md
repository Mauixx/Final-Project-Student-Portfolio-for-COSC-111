# Laboratory Activity #1: Working with Digital Signals

## 📜Description

This activity demonstrates the use of Arduino digital output pins to create a running light effect using multiple LEDs. It highlights how digital signals can be used to control hardware components sequentially, which is a fundamental concept in Arduino-based and IoT-related systems.

## 🖇️Objectives

1. Review Arduino as a device for IoT systems implementation.
2. Discuss digital signals and their implementation in an Arduino circuit.

## ⚓Concepts

* Arduino digital output control using `digitalWrite()`
* Digital signal states (HIGH and LOW)
* Sequential logic in embedded systems
* Timing control using the `delay()` function
* Basic LED interfacing with Arduino

## ⚙️System Overview

The system consists of an Arduino board connected to five LEDs using digital pins 8 to 12. The Arduino program activates the LEDs sequentially from pin 12 down to pin 8 to create a running light effect. After all LEDs are turned on, the same sequence is used to turn them off. A one-second delay between each step controls the speed of the running light pattern.

## 💡Conclusion

This activity reinforces essential Arduino programming concepts, particularly digital signal control and sequential execution. By implementing a running light circuit, students gain practical experience in controlling multiple outputs, which is a foundational skill for developing more complex IoT and embedded system applications.


## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `lab1_activity.ino` | Arduino sketch for configuring digital pins and running the sequential LED ON/OFF logic |
| `lab1_breadboard_diagram.png` | Breadboard diagram showing Arduino connections to LEDs and resistors |
```


