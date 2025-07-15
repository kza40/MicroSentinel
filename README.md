# Tamper-Evident Embedded System

This project is a tamper-evident embedded system built on an Arduino Nano, designed to detect and log unauthorized physical access. It combines motion and magnetic sensors with a lightweight embedded firmware to securely store events, making it ideal for low-power, space-constrained environments.

## 🔧 Features

- Tamper detection using magnetic and motion-based sensing
- Persistent event logging via I2C-connected memory
- Serial interface for controlled event access
- Low-power footprint suitable for mobile deployments

> ✳️ *Some detection thresholds, filtering logic, and response behaviors have been intentionally omitted.*

## 🧰 Hardware Components

| Component           | Notes                                           |
|---------------------|-------------------------------------------------|
| Arduino Nano        | 8-bit ATmega328P microcontroller (core unit)    |
| MPU6050             | 6-axis motion sensor (I2C)                      |
| Reed Switch         | Passive magnetic tamper detection               |
| AT24C32 EEPROM      | I2C EEPROM used for event logging               |
| Breadboard + Wires  | Prototyping environment                         |
| Power Supply        | Dependant on the environment                    |


## 🧠 Software Overview

- **Language**: Embedded C++ (Arduino core)
- **Core Libraries**:
  - `Wire.h` 
  - `EEPROM_I2C` 
  - `MPU6050.h` 
  - `RTClib` — 
  - `Serial` / `SoftwareSerial`



