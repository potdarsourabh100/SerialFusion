# 🚀 SerialFusion

![3D Render](/Image/SerialFusion.png)

*Universal Isolated USB-to-UART / ESP32 Programmer / RS485 / RS232 Converter*

---

## 📖 Overview

**SerialFusion** is a professional-grade isolated USB communication and programming tool designed for embedded engineers, makers, students, and industrial automation developers.

The board combines multiple serial communication interfaces into a single compact device:

* USB ↔ UART (TTL/CMOS)
* ESP32 Auto Programmer
* USB ↔ RS485 Converter
* USB ↔ RS232 Converter

At its core is the reliable **CH340K USB-UART bridge**, combined with digital isolation, isolated power, industrial-grade transceivers, and ESP32 auto-programming support.

Unlike typical USB-TTL adapters, SerialFusion provides electrical isolation, industrial communication interfaces, visual status indicators, and user-friendly connectors suitable for both development and field deployment.

---

## ✨ Features

### USB-C Connectivity

* USB Type-C interface
* ESD-protected USB data lines
* Modern reversible connector
* Bus-powered operation

### Isolated UART Interface

* CH340K USB-UART bridge
* ISO7721 digital isolation
* Complete galvanic isolation between PC and target hardware
* Protection against ground loops and industrial noise

### Isolated Power Supply

* MEJ1S0505SC isolated DC-DC converter
* Independent isolated target-side supply
* Low-noise 3.3V regulation using MIC5219

### ESP32 Programming Support

* Automatic bootloader entry
* RTS → EN control
* DTR → IO0 control
* Compatible with ESP-IDF
* Compatible with Arduino IDE
* Manual BOOT and RESET pushbuttons

### RS485 Interface

* ISL3172E industrial RS485 transceiver
* Half-duplex communication
* Selectable onboard 120Ω termination resistor
* Suitable for:

  * Modbus RTU
  * EST-RBUS16
  * Custom industrial protocols
  * Multi-drop networks

### RS232 Interface

* MAX3232 RS232 transceiver
* Standard DB9 connector
* Full voltage-level conversion
* Legacy equipment compatibility

### Debugging Features

* Dedicated UART debug header
* TX activity LED
* RX activity LED
* Power indicator LED
* Clearly labeled pinout

### User-Friendly Design

* Color-coded silkscreen labels
* Compact PCB layout
* Ground-pour optimized routing
* Easy access connectors
* Professional assembly-friendly footprint selection

---

## 🔌 Interfaces

### ESP32 Programming Header

| Pin | Function     |
| --- | ------------ |
| TX  | UART TX      |
| RX  | UART RX      |
| EN  | ESP32 Reset  |
| IO0 | ESP32 Boot   |
| 3V3 | Target Power |
| GND | Ground       |

Supports automatic firmware upload without manual button presses.

---

### UART Debug Header

| Pin | Function |
| --- | -------- |
| TX  | UART TX  |
| RX  | UART RX  |
| 3V3 | Supply   |
| GND | Ground   |

Ideal for debugging microcontrollers and embedded systems.

---

### RS485 Connector

| Pin | Function |
| --- | -------- |
| A   | RS485 A  |
| B   | RS485 B  |

Features selectable onboard termination resistor.

---

### RS232 Connector

Standard DB9 serial interface for legacy equipment and industrial devices.

---

## 🏗 Architecture

PC USB

↓

USB-C

↓

CH340K USB-UART

↓

ISO7721 Isolation

↓

┌─────────────┬─────────────┬─────────────┐

│ UART Debug │ ESP32 Prog │ Industrial │

│ Interface │ Interface │ Interfaces │

│ │ │ │

│ │ │ ├── RS485

│ │ │ └── RS232

└─────────────┴─────────────┴─────────────┘

---

## ⚡ Power Architecture

USB 5V

↓

MEJ1S0505SC

(Isolated DC-DC)

↓

MIC5219-3.3

↓

Isolated 3.3V Rail

This architecture provides protection against:

* Ground loops
* Industrial noise
* USB port damage
* Common-mode voltage issues

---

## 🧪 Typical Applications

### Embedded Development

* ESP32 programming
* STM32 debugging
* RP2040 development
* AVR programming
* UART monitoring

### Industrial Automation

* Modbus RTU testing
* PLC communication
* RS485 network diagnostics
* Protocol development
* Field commissioning

### Education & Learning

* Serial communication experiments
* Embedded systems labs
* Industrial communication training

---

## 🔥 Project Status

Current Stage:

**Prototype Validation**

Roadmap:

* [x] Schematic Design
* [x] PCB Layout
* [ ] Prototype Assembly
* [ ] Functional Testing
* [ ] Firmware Validation
* [ ] Production Release

---

## ❤️ Author

### EmbSysTech Innovations

**Bytes of Innovations**

Designed with passion for Embedded Systems, Industrial Electronics, and Open Hardware.

---

## ⭐ Support

If you like this project:

⭐ Star the repository

🍴 Fork the project

📢 Share with makers, students, and engineers

☕ Help spread the word about open hardware development
