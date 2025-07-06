# 🌍 Earthquake & Smoke Detection System Using Arduino 🚨🔥


---

## 📌 Project Overview

### 1. Purpose  
Design a **real-time alert system** to detect seismic activity 🌐 and smoke 🔥, providing instant alerts via sound, lights, and display for enhanced safety.

---

### 2. Key Features  
- 🌍 Detects earthquake vibrations using a vibration sensor  
- 🌫️ Monitors smoke levels with MQ-2 smoke sensor  
- 🔊 Audible alerts with buzzer & MP3 audio via DFPlayer Mini  
- 💻 Displays status & alerts on 20x4 I2C LCD screen  
- 🔴 Red LED for alerts, 🟢 Green LED for normal status  
- 💸 Low-cost, reliable, scalable Arduino Uno-based design

---

### 3. Components  
| Component               | Use / Description                          |
|------------------------|--------------------------------------------|
| Arduino Uno            | Microcontroller                            |
| Vibration Sensor       | Detects seismic vibrations                 |
| MQ-2 Smoke Sensor      | Measures smoke concentration (analog)     |
| LiquidCrystal_I2C (20x4) | Displays messages and alerts                |
| DFRobot DFPlayer Mini  | Plays alert sounds (MP3)                    |
| SoftwareSerial         | Serial comm. with DFPlayer                  |
| Buzzer                 | Loud alarm sounds                           |
| Red & Green LEDs       | Alert (red) and normal (green) indicators  |
| Speaker                | Audio output                               |
| Jumper Wires, Breadboard | Circuit prototyping                        |

---

### 4. How It Works  
- The **vibration sensor** detects ground movement → triggers red LED, buzzer, LCD alert & earthquake sound 🔊  
- The **smoke sensor** reads air quality → if smoke level > threshold, triggers similar alert with smoke warning sound 🔔  
- When idle, green LED is ON and LCD displays:  
  > **System Monitoring...** 🟢

---

### 5. Objective  
Create a **responsive Arduino prototype** that:  
- Detects earthquakes and smoke reliably 🌍🔥  
- Sends immediate, multi-modal alerts (audio, visual, text)  
- Offers an affordable safety solution for homes, schools & more 🏠🎓

---

### 6. Coding Platform  
- **Arduino IDE**  
- Language: C/C++  
- Libraries used:  
  - `Wire.h` (I2C communication)  
  - `LiquidCrystal_I2C.h` (LCD control)  
  - `SoftwareSerial.h` (MP3 communication)  
  - `DFRobotDFPlayerMini.h` (MP3 control)  

---

### 7. Methods  

**Hardware:**  
- Connect sensors & outputs to Arduino pins  
- LCD uses I2C (SDA = A4, SCL = A5)  
- DFPlayer Mini connected via SoftwareSerial (pins 10 & 11)  

**Software:**  
- `setup()` initializes devices & shows ready message  
- `loop()` monitors sensors continuously  
- Alerts trigger buzzer, LEDs, LCD, and audio playback  
- System resets to monitoring mode after alerts  

---

### 8. Conclusion  
This project delivers a **dual alert system** for earthquake and smoke detection using Arduino. Combining sound, light, and display feedback increases user awareness in emergencies. It sets a foundation for future smart IoT safety systems with remote alerting potential.

---
![Thank You](https://img.shields.io/badge/Thank%20You!-blue?style=flat-square&logo=smile)


