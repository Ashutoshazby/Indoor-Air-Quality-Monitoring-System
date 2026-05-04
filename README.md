# Indoor-Air-Quality-Monitoring-System
Developed an air quality monitoring system using gas sensors and ESP32 for real-time environmental analysis. Implemented threshold-based alert system using buzzer and LED for unsafe air conditions.
# 🌫️ Advanced Indoor Air Quality Monitoring System (ESP32)

## 📌 Overview

This project is an advanced Indoor Air Quality (IAQ) monitoring system built using ESP32, capable of measuring temperature, humidity, particulate matter (PM2.5 & PM10), and gas levels in real time. It calculates AQI (Air Quality Index) and provides alerts for unsafe environmental conditions.

---

## ⚙️ Components Used

* ESP32 / NodeMCU
* PMS5003 Dust Sensor (PM2.5 & PM10)
* MQ Gas Sensor
* DHT22 Temperature & Humidity Sensor
* LED Indicator
* Buzzer
* Jumper Wires & Power Supply

---

## 🔧 Features

* ✅ Real-time monitoring of:

  * Temperature & Humidity (DHT22)
  * PM2.5 and PM10 (PMS Sensor)
  * Gas concentration (MQ Sensor)
* ✅ AQI calculation based on PM2.5 levels
* ✅ Moving average filter for noise reduction
* ✅ Sensor failure handling (fallback values)
* ✅ LED & buzzer alert system for unsafe conditions
* ✅ Serial monitoring dashboard

---

## 🧠 Working Principle

* DHT22 reads environmental temperature and humidity
* PMS sensor provides PM2.5 and PM10 data via serial communication
* MQ sensor reads gas concentration (analog values)
* A moving average filter smooths PM2.5 readings
* AQI is calculated using standard thresholds
* System categorizes air quality (Good → Hazardous)
* Alerts are triggered if AQI or gas levels exceed safe limits

---

## 📊 AQI Classification

| AQI Range | Status                |
| --------- | --------------------- |
| 0–50      | Good                  |
| 51–100    | Moderate              |
| 101–150   | Unhealthy (Sensitive) |
| 151–200   | Unhealthy             |
| 201+      | Hazardous             |

---

## ⚠️ Alert Conditions

* AQI > 150 → LED & Buzzer ON
* Gas Level > Threshold → Alert Triggered

---

## 🛠️ Technical Highlights

* Moving Average Filtering for PM2.5 stabilization
* Serial communication with PMS sensor
* Fault-tolerant design using last valid sensor values
* Modular code structure with reusable functions
* Real-time embedded system implementation

---

## 🚀 Future Improvements

* Add WiFi dashboard using ESP32
* Integrate cloud storage (Firebase / Thingspeak)
* Mobile app notifications
* Add OLED/LCD display
* GPS-based outdoor air quality tracking

---

## 📎 Notes

* Ensure proper calibration of MQ sensor for accurate readings
* PMS sensor requires stable power supply
* Delay timings are optimized for sensor reliability

---

## 🧑‍💻 Author

**Ashutosh Tiwari**
Full Stack Developer | IoT & AI Enthusiast
