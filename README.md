# 🔧 Arduino IDE Windows Driver Setup

This repository provides the required **Windows USB drivers** needed to successfully run **Arduino IDE** and detect Arduino-compatible boards on laptops and PCs.

It helps users fix common problems such as:

- Arduino board not detected
- COM port not appearing
- Upload errors in Arduino IDE
- USB device not recognized

---

## 📌 Overview

Many Arduino-compatible boards (especially ESP32, ESP8266, and clone Arduino boards) require USB-to-Serial drivers before communication with Arduino IDE can work properly.

This package allows users to quickly install the necessary drivers and start programming without configuration issues.

---

## 💻 Supported Operating Systems

- ✅ Windows 10
- ✅ Windows 11

---

## 🔌 Supported Boards

- Arduino Uno (Clone Versions)
- NodeMCU ESP8266
- ESP32 Development Boards
- CH340-based boards
- CP210x USB-to-UART devices

---

## 📦 Included Drivers

- CH340 USB Driver
- CP210x USB Driver

*(Driver requirement depends on your board manufacturer.)*

---

## ⚙️ Installation Guide

### Step 1 — Download Repository

Click **Code → Download ZIP** and extract the folder.

---

### Step 2 — Install Driver

1. Open the driver folder.
2. Right-click the installer file.
3. Select:

Run as Administrator

4. Click **Install** and wait for completion.

---

### Step 3 — Connect Arduino Board

Plug your Arduino or ESP board into your laptop using a USB cable.

Windows will automatically detect the device after driver installation.

---

### Step 4 — Verify in Arduino IDE

1. Open Arduino IDE.
2. Navigate to:

Tools → Port

3. Select the available COM port (example: COM3 / COM4).

---

## ✅ Test the Setup

Upload the Blink example:

File → Examples → Basics → Blink

If the upload is successful, the driver installation is complete.

---

## ❗ Troubleshooting

### COM Port Not Showing
- Reinstall the driver
- Try another USB cable
- Restart Arduino IDE

### Device Not Recognized
- Check Device Manager
- Look under **Ports (COM & LPT)**

You should see:

USB-SERIAL CH340 (COMx)  
or  
Silicon Labs CP210x USB to UART Bridge

---

## 👨‍💻 Maintainer

**Dipendra Mahato**  
IoT Developer | Embedded Systems Engineer

📧 dipendramahato1000@gmail.com  
🌐 https://dipendramahato.netlify.app

---

## 📜 License

This repository is shared for educational and setup assistance purposes to help users configure Arduino IDE easily on Windows systems.
