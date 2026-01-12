# Laboratory Activity #1: Working with Digital Signals

## 📌 Objectives

This laboratory activity aims to:

1. Review **Arduino** as a device for **IoT systems implementation**
2. Understand **digital signals** and their implementation in an **Arduino circuit**

---



## 🔌 Circuit Description

This activity involves creating a **running light circuit** using digital output pins on the Arduino.

* LEDs are connected to **digital pins 8 to 12**
* Each LED is connected in series with a resistor
* The cathode (short leg) of each LED is connected to **GND**

---

## ⚙️ Program Requirements

The Arduino sketch must follow these rules:

* Use **digital pins 8 to 12**
* Create a **running light effect** from pin **12 down to pin 8**
* Delay between LED actions: **1 second**
* Turn **all LEDs ON one by one**
* Then turn **all LEDs OFF one by one**
* Use the `digitalWrite()` function to control the LEDs

---

## 🧠 How It Works

1. The Arduino sets pins **8 to 12** as OUTPUT pins.
2. LEDs turn ON sequentially from **pin 12 to pin 8**, each after a 1-second delay.
3. Once all LEDs are ON, they turn OFF in the same order.
4. The sequence repeats continuously inside the `loop()` function.

---
## 🗂 Files Included
| File Name | Description |
|----------|-------------|
| `lab1_activity.ino` | Arduino sketch containing the logic for configuring digital pins and controlling the LED sequence |
| `lab1_breadboard_diagram.png` | Breadboard diagram illustrating the hardware connections between the Arduino, LEDs, and resistors |
```


