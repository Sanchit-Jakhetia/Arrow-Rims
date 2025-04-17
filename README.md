# 💊 DoseRight - Intelligent Medicine Management System

*By Team: Arrow Rims*

---

## 🧩 Problem Statement

Millions of patients, especially the elderly, struggle to manage complex medicine schedules. Missed doses or overdoses can lead to severe health complications. Existing pillboxes lack automation, remote scheduling, and verification of medicine intake.

**DoseRight** addresses this by providing a **smart, automated medicine dispenser** that not only dispenses medication on time but also tracks consumption, alerts the user, and allows remote management via the cloud.

---

## ⚙️ Tech Stack

### 🚀 Hardware:

- ESP32
- Stepper Motor with ULN2003A Driver
- IR Sensor for medicine detection
- 20x4 LCD Display
- Push Buttons (Up, Down, Select, Back, Manual)
- Buzzer

### 💾 Software:

- Arduino IDE (Firmware development)
- Firebase Realtime Database (Cloud storage)
- NTP Server (Time sync)
- &#x20;CSS, React.js (Website UI)



---

## 🔧 Setup Instructions

### 🔌 Hardware Setup:

1. Assemble the 3-layer dispenser:

   - Bottom: Stepper motor mount
   - Middle: Rotating disk with compartments
   - Top: Fixed top with dispensing hole

2. Connect components to ESP32 as per this pin mapping:

| Component       | ESP32 Pin |
| --------------- | --------- |
| Push 1 (Back)   | D4        |
| Push 2 (Down)   | D18       |
| Push 3 (Up)     | D19       |
| Push 4 (Select) | D23       |
| Push 5 (Manual) | D25       |
| Motor In1       | D13       |
| Motor In2       | D14       |
| Motor In3       | D27       |
| Motor In4       | D26       |
| Buzzer          | D33       |
| IR Sensor       | D35       |
| LCD SDA         | D21       |
| LCD SCL         | D22       |

3. Power the system using a battery or USB supply.

---

### 🖥️ Firmware Setup:

1. Install **Arduino IDE** and required libraries:

   - `WiFi.h`, `Firebase_ESP_Client`, `LiquidCrystal_I2C`, `Wire.h`, `NTPClient`, `WiFiUdp`

2. Flash the firmware from `firmware/DoseRight_ESP32_Code.ino`

---

### 🌐 Website Setup:

1. Open in browser.
2. Connect to Firebase using your project's credentials.
3. Schedule medicines with:
   - Name, Dosage, Frequency, Timing, Tablet Count, Logs, Notification, Refill Notification.

---

### ☁️ Firebase Setup:

1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a project and set up **Realtime Database**
3. Import firebase/doseright-39af2-default-rtdb-users-export (1).json and configure read/write **rules** from rules.json

---

---

### 🏁 Built with Passion for Hackstasy 2025

**Team: Arrow Rims**
