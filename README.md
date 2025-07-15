# Tamper-Evident Embedded System

This project is a tamper-evident embedded system built on an Arduino Nano, designed to detect and log unauthorized physical access. It combines motion and magnetic sensors with a lightweight embedded firmware to securely store events, making it ideal for low-power, space-constrained environments.

## 🔧 Features

- Tamper detection using magnetic and motion-based sensing
- Persistent event logging via I2C-connected memory
- Optional support for time-based tracking
- Serial interface for controlled event access
- Low-power footprint suitable for mobile or battery-backed deployments
- Breadboard-compatible layout for rapid prototyping and modular extension

> ✳️ *Some detection thresholds, filtering logic, and response behaviors have been intentionally omitted.*

## 🧰 Hardware Components

| Component           | Notes                                           |
|---------------------|-------------------------------------------------|
| Arduino Nano        | 8-bit ATmega328P microcontroller (core unit)    |
| MPU6050             | 6-axis motion sensor (I2C)                      |
| Reed Switch         | Passive magnetic tamper detection               |
| AT24C32 EEPROM      | I2C EEPROM used for event logging               |
| DS3231 (optional)   | Real-Time Clock for timestamping                |
| Breadboard + Wires  | Prototyping environment                         |
| Power Supply        | 5V regulated USB or battery                     |


## 🧠 Software Overview

- **Language**: Embedded C++ (Arduino core)
- **Core Libraries**:
  - `Wire.h` 
  - `EEPROM_I2C` 
  - `MPU6050.h` 
  - `RTClib` — 
  - `Serial` / `SoftwareSerial`



