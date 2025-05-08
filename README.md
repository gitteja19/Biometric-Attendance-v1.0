# Biometric-Attendance-v1.0
# 🧠 IoT Biometric Attendance System(IBAS)

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

**IBAS** is a smart, secure, and connected biometric attendance system built using the **ESP8266**, **Adafruit Fingerprint Sensor**, and **Google Sheets API**. It enables contactless authentication and real-time attendance logging via enterprise Wi-Fi and Google Sheets integration, tailored for educational environments.

---

## 🚀 Features

- **🔒 Biometric Authentication**  
  Secure fingerprint-based student verification using Adafruit Fingerprint Sensor.

- **📡 Wi-Fi Connectivity (Eduroam Compatible)**  
  Connects via WPA2-Enterprise (Eduroam) using custom certificate-based login.

- **📊 Real-Time Google Sheets Logging**  
  Uploads attendance data to Google Sheets instantly via a custom `GAS_ID`.

- **🧠 EEPROM Storage**  
  Stores and verifies up to 1000 student roll numbers in EEPROM for persistent tracking.

- **📟 OLED Visual Feedback**  
  Displays real-time system states like "Wi-Fi Connected", "Scan Success", and error animations.

- **🔉 Keypad & Buzzer Integration**  
  Keypad-based controls with buzzer feedback for scan success, failure, or system messages.

---

## 🔧 Hardware Used

- **ESP8266 NodeMCU **  
- **Adafruit Fingerprint Sensor**  
- **Adafruit SSD1306 OLED (128x64)**  
- **Adafruit MCP23X17 GPIO Expander**  
- **4x4 Matrix Keypad**  
- **SD Card Module**
- **Buzzer**

---

## 🛠 Tech Stack

- **Language**: C++ (Arduino)
- **Libraries**:  
  - `Adafruit_Fingerprint`  
  - `Adafruit_GFX` & `Adafruit_SSD1306`  
  - `Adafruit_MCP23X17`  
  - `ESP8266WiFi` + `wpa2_enterprise.h`  
  - `EEPROM`, `Wire`, `SPI`, `SD`  

---
## 📦 Project Structure

```
.
├── main.ino                     # Main source code
├── TRIGGER_WIFI.h               # Wi-Fi authentication config
├── TRIGGER_GOOGLESHEETS.h       # Google Sheets API interface
├── assets/                      # Bitmap images for OLED feedback
└── data/                        # EEPROM and SD logs (optional)
```
---

## 🖥 Sample OLED Screens

- 🟢 Wi-Fi Connected  
- 🟡 Fingerprint Scanning...  
- ✅ Fingerprint Matched  
- ❌ Invalid Fingerprint  
- 🚫 Access Denied

---

## 🔐 Security Features

- WPA2-Enterprise Eduroam login with username & password  
- Fingerprint template-based matching (no raw data transfer)  
- EEPROM-based ID validation to prevent spoofing  
- Secure admin mode

---

## 📈 Future Enhancements

- Role-based admin panel over Bluetooth  
- Encrypted storage of attendance logs  
- Multi-factor authentication (e.g., PIN + biometric)  
- Integration with ERP platforms like Moodle or SAP

---

## 🧑‍🏫 Guide

**Prof. Nagaveni – IIT Dharwad**  
Faculty Mentor and Technical Advisor

---

## 📄 License

This project is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). For educational and non-commercial use only.
