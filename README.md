# 🌍 AEROQUANT - IoT Based Air Quality & Environment Monitoring System

AEROQUANT is an IoT-based real-time air quality and environmental monitoring system built using ESP32, DHT11, MQ135, and Blynk Cloud.

The system continuously monitors:

- 🌡 Temperature
- 💧 Humidity
- 🌫 Air Quality Index (AQI)

Sensor data is displayed locally on a 16x2 I2C LCD and remotely through the Blynk IoT dashboard. A lightweight machine learning model running on the ESP32 predicts AQI using multiple environmental parameters for improved accuracy.

---

## 🚀 Features

✅ Real-time Temperature Monitoring

✅ Real-time Humidity Monitoring

✅ Air Quality Monitoring using MQ135

✅ ESP32 Wi-Fi Connectivity

✅ Blynk Cloud Dashboard Integration

✅ Local LCD Display

✅ AQI Classification System

✅ Automatic Air Quality Alerts

✅ Lightweight Edge AI AQI Prediction

---

## 🛠 Hardware Components

| Component | Quantity |
|------------|-----------|
| ESP32 DevKit V1 | 1 |
| DHT11 Sensor | 1 |
| MQ135 Gas Sensor | 1 |
| 16x2 LCD Display | 1 |
| I2C LCD Module | 1 |
| Breadboard | 1 |
| Jumper Wires | As Required |

---

## 💻 Software & Libraries

- Arduino IDE
- Blynk IoT Platform
- WiFi.h
- BlynkSimpleEsp32.h
- DHT.h
- LiquidCrystal_I2C.h

---

## ⚙ System Architecture

MQ135 + DHT11 Sensors
        ↓
      ESP32
        ↓
 Machine Learning AQI Model
        ↓
 AQI Classification
        ↓
 LCD Display + Blynk Cloud
        ↓
 Mobile Alerts

---

## 📊 AQI Categories

| AQI Range | Category |
|------------|-----------|
| 0 - 99 | VERY GOOD |
| 100 - 199 | GOOD |
| 200 - 299 | MODERATE |
| 300 - 399 | POOR |
| 400+ | VERY POOR |

---

## 📱 Blynk Dashboard

Virtual Pins:

| Pin | Data |
|------|------|
| V0 | Raw AQI |
| V1 | Predicted AQI |
| V2 | Temperature |
| V3 | Humidity |
| V4 | AQI Category |

---

## 🧠 Embedded Machine Learning Model

The AQI prediction model uses:

- MQ135 Sensor Voltage
- Temperature
- Humidity

Formula:

AQI = ((0.60 × Voltage) + (0.25 × Temperature) + (0.15 × Humidity)) × 500

---

## 📸 Project Images

### Circuit Diagram
(Add Image Here)

### Hardware Setup
(Add Image Here)

### Blynk Dashboard
(Add Screenshot Here)

---

## 🔮 Future Improvements

- MQTT Integration
- TensorFlow Lite Model
- PM2.5 / PM10 Sensors
- Solar Powered Deployment
- OTA Firmware Updates
- Historical Data Analytics

---

## 👨‍💻 Authors

**Kinara Patel**  
ICT Department, PDEU

**Meet K. Vaswani**  
ICT Department, PDEU

---

## ⭐ If you like this project, consider giving it a star!
