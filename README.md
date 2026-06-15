# Smart Plant Monitoring and Automatic Irrigation System using NodeMCU and Blynk IoT

## Overview

This project is an IoT-based Smart Plant Monitoring System developed using NodeMCU ESP8266 and Blynk Cloud. The system continuously monitors soil moisture, temperature, humidity, and motion around the plant area while allowing remote monitoring and control through the Blynk mobile application.

The project helps automate irrigation and provides real-time environmental monitoring to improve plant health and reduce water wastage.

---

## Features

* Real-time Soil Moisture Monitoring
* Temperature Monitoring using DHT11 Sensor
* Humidity Monitoring using DHT11 Sensor
* PIR Motion Detection
* Automatic Water Pump Control
* Manual Pump Control through Blynk App
* LCD Display for Live Sensor Data
* Remote Monitoring using Blynk Cloud
* IoT-based Smart Irrigation System

---

## Components Used

| Component                           | Quantity    |
| ----------------------------------- | ----------- |
| NodeMCU ESP8266                     | 1           |
| DHT11 Temperature & Humidity Sensor | 1           |
| Soil Moisture Sensor                | 1           |
| PIR Motion Sensor                   | 1           |
| Relay Module                        | 1           |
| Water Pump                          | 1           |
| 16x2 I2C LCD Display                | 1           |
| Jumper Wires                        | As Required |
| Power Supply                        | 1           |

---

## Pin Connections

| Component            | NodeMCU Pin |
| -------------------- | ----------- |
| Relay Module         | D3          |
| Push Button          | D7          |
| Soil Moisture Sensor | A0          |
| PIR Sensor           | D5          |
| DHT11 Sensor         | D4          |
| LCD SDA              | D2          |
| LCD SCL              | D1          |

---

## Working Principle

1. Soil moisture sensor measures the water content in soil.
2. Temperature and humidity values are collected from the DHT11 sensor.
3. PIR sensor detects motion near the plant area.
4. Sensor values are displayed on the LCD screen.
5. Sensor readings are sent to the Blynk IoT Dashboard.
6. Users can remotely monitor plant conditions through the Blynk mobile app.
7. The relay controls the water pump automatically or manually through Blynk.
8. Notifications are generated when motion is detected.

---

## Blynk Virtual Pins

| Virtual Pin | Function             |
| ----------- | -------------------- |
| V0          | Temperature          |
| V1          | Humidity             |
| V3          | Soil Moisture        |
| V5          | Motion Detection LED |
| V6          | PIR Enable/Disable   |
| V12         | Pump Control         |

---

## Software Requirements

* Arduino IDE
* ESP8266 Board Package
* Blynk IoT Platform
* CP2102 USB Driver
* Required Arduino Libraries

---

## Required Libraries

Install the following libraries from Arduino Library Manager:

```text
Blynk
ESP8266WiFi
DHT Sensor Library
LiquidCrystal I2C
```

---

## Arduino IDE Setup

### Add Board Manager URLs

File → Preferences → Additional Board Manager URLs

```text
https://arduino.esp8266.com/stable/package_esp8266com_index.json
https://dl.espressif.com/dl/package_esp32_index.json
```

### Install Boards

* ESP8266 by ESP8266 Community
* ESP32 by Espressif Systems

### Select Board

```text
Tools → Board → ESP8266 Boards → NodeMCU 1.0
```

### Select Port

```text
Tools → Port → Select Connected COM Port
```

---

## Configuration

Update the following credentials before uploading the code:

```cpp
char auth[] = "YOUR_BLYNK_AUTH_TOKEN";
char ssid[] = "YOUR_WIFI_NAME";
char pass[] = "YOUR_WIFI_PASSWORD";
```

---


---

## Applications

* Smart Agriculture
* Greenhouse Monitoring
* Home Gardening
* Automated Irrigation Systems
* IoT-based Farming Solutions
* Environmental Monitoring

---

## Future Enhancements

* Mobile Notifications for Low Soil Moisture
* AI-based Watering Prediction
* Weather API Integration
* Cloud Data Analytics
* Solar Powered Irrigation System
* Multiple Plant Monitoring Support

---

## Results

The system successfully:

* Monitors soil moisture in real-time
* Displays environmental conditions on LCD
* Controls water pump remotely
* Detects motion using PIR sensor
* Sends sensor data to Blynk Cloud
* Enables smart irrigation management

---

## Author

Kavin Kumar S

B.Tech Artificial Intelligence and Data Science

Interested in IoT, Artificial Intelligence, Embedded Systems, Computer Vision, and Industrial Automation.

---

## License

This project is developed for educational and research purposes.
