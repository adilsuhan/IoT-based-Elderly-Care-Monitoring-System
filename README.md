# Elderly Care Monitoring System

An IoT-based Elderly Care Monitoring System designed to improve the safety and well-being of senior citizens. The system uses an ESP32 microcontroller with motion and GPS sensors to detect falls, monitor location in real time, provide medicine reminders, and display live data through a web dashboard.

---

##  Project Overview

The Elderly Care Monitoring System is a smart healthcare solution that continuously monitors an elderly person's movement and location. Using an MPU6050 accelerometer and gyroscope, the system detects falls and immediately activates an emergency buzzer. A GPS module provides real-time location tracking, while an ESP32 hosts a web dashboard that allows caregivers to monitor the user's status remotely over Wi-Fi. Additionally, a medicine reminder helps users maintain their daily medication schedule.

---

##  Features

-  Real-time fall detection
-  Live GPS location tracking
-  Emergency buzzer alert
-  Medicine reminder
-  ESP32 hosted web dashboard
-  Wi-Fi based monitoring
-  Remote caregiver access
-  Low-cost IoT healthcare solution

---

##  Hardware Components

- ESP32 Development Board
- MPU6050 Accelerometer & Gyroscope
- GPS Module (NEO-6M)
- Active Buzzer
- Push Button
- Breadboard
- Jumper Wires
- USB Cable / Power Supply

---

##  Software & Technologies

- Arduino IDE
- ESP32 Board Package
- Embedded C++
- HTML
- CSS
- JavaScript
- Wi-Fi
- TinyGPS++
- Adafruit MPU6050 Library
- WebServer Library

---

##  System Workflow

1. ESP32 initializes all connected sensors.
2. MPU6050 continuously monitors body movement.
3. GPS module updates the user's current location.
4. If abnormal acceleration exceeds the threshold:
   - Fall is detected.
   - Emergency buzzer is activated.
5. The user can stop the buzzer using the push button if the alarm is false.
6. Medicine reminders are generated at predefined intervals.
7. ESP32 hosts a live web dashboard displaying:
   - GPS Coordinates
   - Fall Detection Status
   - Buzzer Status
   - Medicine Reminder
8. Caregivers can monitor the elderly person remotely through the dashboard.

---

## System Architecture

```
MPU6050 ──┐
          │
GPS ──────┤
          │
Button ───┤
          ▼
        ESP32
          │
          ├── Web Dashboard
          ├── Buzzer Alert
          └── Wi-Fi Monitoring
```

---

##  Hardware Connections

### MPU6050

| Pin | ESP32 |
|-----|--------|
| VCC | 3.3V |
| GND | GND |
| SDA | GPIO21 |
| SCL | GPIO22 |
| INT | GPIO19 |

### GPS Module

| Pin | ESP32 |
|-----|--------|
| VCC | 5V |
| GND | GND |
| TX | GPIO16 |
| RX | GPIO17 |

### Buzzer

| Pin | ESP32 |
|-----|--------|
| + | GPIO18 |
| - | GND |

---

##  Project Structure

```
Elderly-Care-Monitoring-System/
│
├── code/
│   └── elderly_care.ino
│
├── images/
│   ├── hardware.jpg
│   ├── dashboard.png
│   ├── flowchart.png
│   └── architecture.png
│
├── report/
│   └── IOT_Project.pdf
│
├── README.md
└── LICENSE
```

---

##  Results

- Successfully detected fall events using the MPU6050 sensor.
- Displayed real-time GPS location on the web dashboard.
- Activated emergency buzzer during fall detection.
- Generated timely medicine reminders.
- Hosted a responsive web dashboard using the ESP32.
- Enabled reliable real-time monitoring over Wi-Fi.

---

## Future Enhancements

- Firebase Cloud Integration
- Mobile Application
- SMS & Email Notifications
- Heart Rate Monitoring
- SpO₂ Monitoring
- Body Temperature Sensor
- Cloud Data Storage
- AI-Based Fall Prediction
- Emergency Contact Notifications

---

##  Applications

- Home Healthcare
- Elderly Care Centers
- Hospitals
- Assisted Living Facilities
- Smart Healthcare Systems
- Remote Patient Monitoring

---

## 🌟 Support

If you found this project useful, don't forget to **⭐ Star** this repository!
