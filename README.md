# 🅿️ IoT-Based Smart Parking System with RFID Authentication

A secure, automated, and real-time monitoring parking system built using Arduino, RFID, and IoT technologies.

---

## 📌 Overview

This project presents a cost-effective and scalable smart parking solution that integrates **RFID-based authentication**, **real-time slot monitoring**, and **IoT-based remote management**. The system ensures only authorized vehicles can enter, monitors parking slot availability using IR sensors, and provides live updates via the Blynk IoT platform.

---

## 🎯 Key Features

- **RFID Authentication**: Secure entry and exit using MFRC522 RFID modules.
- **Real-Time Slot Monitoring**: IR sensors detect vehicle presence and update slot status.
- **Automatic Gate Control**: Servo motors control entry and exit gates.
- **Safety Alerts**: Buzzer alerts for unauthorized access, smoke (MQ2), and alcohol detection (MQ3).
- **IoT Dashboard**: Live parking status on Blynk app via ESP32.
- **LCD Display**: Shows slot availability and system messages.

---

## 🛠️ System Architecture

### Components Used

| Component         | Quantity | Purpose                          |
|-------------------|----------|----------------------------------|
| Arduino Uno       | 1        | Main microcontroller             |
| ESP32             | 1        | Wi-Fi and IoT communication      |
| MFRC522 RFID      | 2        | Entry/exit authentication        |
| IR Sensor         | 4        | Slot occupancy detection         |
| Servo Motor       | 2        | Gate control                     |
| MQ2 Sensor        | 1        | Smoke detection                  |
| MQ3 Sensor        | 1        | Alcohol detection                |
| I2C LCD           | 1        | Status display                   |
| Buzzer            | 1        | Alert system                     |

### Block Diagram

```
RFID → Arduino Uno → Servo (Gate Control)
IR Sensors → ESP32 → Blynk IoT Dashboard
LCD & Buzzer → Alerts & Status
```

---

## 🔧 Implementation

### Communication Protocols

- **SPI**: Used for RFID module communication.
- **UART**: Used for Arduino-ESP32 serial communication.
- **Wi-Fi**: ESP32 connects to Blynk cloud for real-time updates.

### Circuit Design

The system integrates multiple sensors and actuators powered via Arduino’s 3.3V and 5V pins. A mobile hotspot is used for reliable Wi-Fi connectivity.

---

## 💡 Challenges & Solutions

| Challenge | Solution |
|-----------|----------|
| Voltage mismatch between 3.3V and 5V components | Used Arduino’s built-in 3.3V and 5V pins |
| Unreliable Wi-Fi | Used mobile hotspot for consistent connectivity |
| RFID sensor not reading | Powered via 5V instead of 3.3V for sufficient current |

---

## 📊 Results

- ✅ RFID authentication works seamlessly with servo gate control.
- ✅ IR sensors provide 100% accuracy in slot detection.
- ✅ Real-time Blynk dashboard updates.
- ✅ Unauthorized access triggers buzzer alerts.

---

## 🌱 Sustainability & Impact

- **Low Power Design**: Uses energy-efficient microcontrollers and sensors.
- **Modularity**: Components can be reused or upgraded.
- **Scalable**: Can be extended with billing, notifications, or license plate recognition.

---

## 👥 Team Contributions

| Name | ID | Role |
|------|----|------|
| Syed Faysel Ahammad Rajo | 21101078 | Circuit building, Arduino coding |
| Mehedi Hasan Shahed | 21301436 | Hardware design, ESP32 coding |
| Zarin Tasnim Raisa | 21301022 | Circuit building, report writing |


---

## 🔗 References

- Mohammed & Wei (n.d.). *Study on Automated Car Parking System Based on Microcontroller*.
- Jusat et al. (2021). *Critical review in smart car parking management systems*.
- Shahin et al. (2023). *Automatic Car Parking System Using Arduino*.

---

## 📬 Contact

For queries or collaboration, feel free to reach out to the team members via their university emails.

---
**BRAC University**  
**CSE360: Computer Interfacing**  
**Group 06 | Section 05**  
**September 2025**
