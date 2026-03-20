# 🦠 Box-Covid

> Remote monitoring system for COVID-19 patients using IoT, Cloud, and Mobile technologies.

## 📌 Overview

**Box-Covid** is an intelligent healthcare system designed to help doctors remotely monitor and manage patients infected with COVID-19.

The system reduces direct contact, minimizes infection risk, and provides real-time health insights through connected devices and a cross-platform application.

---

## 🚀 Features

- 📡 Real-time patient monitoring (temperature, heart rate, oxygen saturation)
- 🌡️ Environmental monitoring (humidity & ambient temperature)
- ☁️ Cloud-based data storage (AWS)
- 👨‍⚕️ Doctor dashboard for:
  - Monitoring patients
  - Writing prescriptions
  - Communication with patients
- 👨‍👩‍👧 Patient & family access:
  - Health dashboard
  - Medications
  - Doctor recommendations

---

## 🏗️ System Architecture

The project is composed of **3 main components**:

### 1️⃣ Smart Medical Box (Hardware)
- Collects patient and environmental data using sensors
- Sends data to the cloud

**Technologies:**
- Raspberry Pi 3B+
- ESP32
- Sensors:
  - Body Temperature
  - Heart Rate
  - Oxygen Saturation (SpO2)
  - Ambient Temperature
  - Humidity
- Custom PCB

---

### 2️⃣ Cloud Infrastructure (AWS)
- Stores and processes incoming data
- Connects hardware with the application

**Services:**
- AWS Cloud (Data Storage & Communication)

---

### 3️⃣ Cross-Platform Application
- Enables remote interaction between doctors and patients

**Features:**
- Patient monitoring dashboard
- Prescription management
- Communication system

**Technologies:**
- Apache Cordova
- Node.js
- MySQL
- phpMyAdmin

---

## 🛠️ Tech Stack

### 🔵 Hardware
- Raspberry Pi
- ESP32
- Embedded Sensors
- Arduino IDE

### 🔵 Software
- Node.js
- Apache Cordova
- Node-RED
- MySQL

### 🔵 Cloud
- AWS

---

## 📂 Project Structure

```
.
├── hooks/
├── node_modules/
├── platforms/
├── plugins/
├── res/
├── www/              # Application frontend
├── config.xml
├── package.json
└── README.md
```

## ⚙️ Installation & Setup

### Prerequisites
- Node.js
- Apache Cordova
- MySQL
- Arduino IDE (for hardware setup)

### Steps

```bash
# Clone the repository
git clone https://github.com/your-username/Covid-19_App.git

# Navigate to project
cd Covid-19_App

# Install dependencies
npm install

# Run the application
cordova run browser
