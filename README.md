# 💧 Water Level Monitoring System using ESP32

## 📌 Overview

This project is an **IoT-based Water Level Monitoring System** built using **ESP32**, **Ultrasonic Sensor**, **LED indicators**, and a **Buzzer**.

It measures the water level in a tank and indicates whether the level is **Low, Medium, or High** using LEDs and sound alerts.

---

## ⚙️ Features

* Water level detection using ultrasonic sensor
* Multi-level indication (Low, Medium, High)
* LED indicators for each level
* Buzzer alert for high water level
* Real-time monitoring via Serial output

---

## 🧠 Project Description

This system uses an **ultrasonic sensor** to measure the distance between the sensor and the water surface, and determines the water level based on that distance.

---

### 🔹 Ultrasonic Sensor Working

* **Trigger pin** sends ultrasonic waves

* **Echo pin** receives reflected waves

* Time taken is used to calculate distance

* Short distance → High water level

* Large distance → Low water level

---

### 🔹 Water Level Detection Logic

Based on distance:

* **Distance > 20 cm → Low Water Level**
* **Distance < 10 cm → Medium Water Level**
* **Else → High Water Level**

---

### 🔹 LED Indicators

* 🔵 Low Level → Low LED ON
* 🟡 Medium Level → Medium LED ON
* 🔴 High Level → High LED ON

---

### 🔹 Buzzer Alert

* Buzzer activates when water level is **High**
* Acts as an overflow warning system

---

### 🔹 Serial Monitoring

Displays:

* Distance in cm
* Current water level status

Example:

* `"Water Level: Low"`
* `"Water Level: Medium"`
* `"Water Level: High"`

---

## 🔄 Working Flow

1. ESP32 triggers ultrasonic sensor
2. Distance is measured
3. Water level is calculated based on distance
4. Corresponding LED is activated
5. If water level is high:

   * Buzzer turns ON
6. Status is printed on Serial Monitor

---

## 🧠 Learning Outcomes

* Interfacing ultrasonic sensors with ESP32
* Measuring distance using pulse timing
* Multi-condition logic implementation
* Using multiple LEDs for indication
* Designing real-time monitoring systems

---

## 🚀 Future Enhancements

* Display level on LCD/OLED
* IoT monitoring (mobile/web dashboard)
* Automatic motor control (water pump)
* SMS/Telegram alerts
* Data logging to cloud

---

## 👩‍💻 Author

**Amrutha D N**
