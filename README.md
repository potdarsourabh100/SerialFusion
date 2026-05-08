# 🔌 USB to TTL / RS485 / RS232 Converter

> A compact multi-protocol USB communication tool based on CH340K, MAX232 & MAX485 for embedded development, industrial communication, debugging, and automation projects.

![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-blue)
![Status](https://img.shields.io/badge/status-Development-orange)
![PCB](https://img.shields.io/badge/PCB-KiCad-success)

---

# ✨ Features

✅ USB to UART (TTL)  
✅ USB to RS485  
✅ USB to RS232  
✅ CH340K USB-UART Bridge  
✅ MAX485 Half-Duplex RS485 Transceiver  
✅ MAX232 RS232 Level Converter  
✅ TX/RX Status LEDs  
✅ Compact PCB Design  
✅ ESD & Protection Circuitry  
✅ Selectable Communication Modes  
✅ 3.3V / 5V Compatible Logic Support  
✅ Screw Terminal Connectivity for RS485  
✅ Plug & Play USB Driver Support

---

# 📷 Project Preview

## 3D PCB Render

_Add PCB image here_

```text
/images/pcb_render.png
```

## Schematic Preview

_Add schematic image here_

```text
/images/schematic.png
```

---

# 🧠 Why This Project?

Most USB communication adapters support only one protocol.

This project combines:

- TTL UART
- RS485
- RS232

into a **single compact hardware tool** useful for:

- Embedded engineers
- Industrial automation
- PLC communication
- Arduino/STM32 debugging
- Modbus testing
- Firmware flashing
- Serial monitoring

---

# 🛠️ Hardware Used

| Component | Description |
|----------|-------------|
| CH340K | USB to UART IC |
| MAX485 | RS485 Transceiver |
| MAX232 | RS232 Level Shifter |
| AMS1117 | Voltage Regulator |
| USB Type-C / Micro USB | USB Interface |
| LEDs | TX/RX/Power Indicators |
| TVS Diodes | ESD Protection |
| Terminal Blocks | RS485 Connectivity |

---

# ⚙️ Communication Modes

| Mode | Interface | Usage |
|------|-----------|-------|
| TTL UART | TX/RX/GND | MCU Debugging |
| RS485 | A/B/GND | Industrial Communication |
| RS232 | TX/RX/GND | Legacy Serial Devices |

---

# 🔄 Block Diagram

```text
                 +----------------+
USB ---> CH340K--| UART Interface |
                 +--------+-------+
                          |
        +-----------------+------------------+
        |                                    |
   +----+----+                         +-----+-----+
   | MAX485  |                         |  MAX232   |
   | RS485   |                         |  RS232    |
   +----+----+                         +-----+-----+
        |                                    |
      A / B                              TX / RX
```

---

# 🔌 Pinout

## TTL Header

| Pin | Description |
|-----|-------------|
| TXD | UART TX |
| RXD | UART RX |
| GND | Ground |
| VCC | 5V/3.3V |

---

## RS485 Terminal

| Pin | Description |
|-----|-------------|
| A | RS485 A |
| B | RS485 B |
| GND | Ground |

---

## RS232 DB9

| Pin | Description |
|-----|-------------|
| TX | Transmit |
| RX | Receive |
| GND | Ground |

---

# 📁 Project Structure

```text
USB-MultiProtocol-Converter/
│
├── Hardware/
│   ├── Schematic/
│   ├── PCB/
│   ├── Gerber/
│   └── BOM/
│
├── Firmware/
│
├── Images/
│
├── Docs/
│
└── README.md
```

---

# 🚀 Getting Started

## 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/USB-MultiProtocol-Converter.git
```

---

## 2️⃣ Open PCB Files

Recommended Software:

- KiCad
- EasyEDA
- Altium Designer

---

## 3️⃣ Assemble PCB

Solder all components carefully according to schematic.

---

## 4️⃣ Install USB Driver

### Windows

Install CH340 Driver.

### Linux

Drivers are usually pre-installed.

### macOS

Install compatible CH340 USB drivers.

---

# 🧪 Testing

## TTL Test

- Connect TX ↔ RX
- Open serial monitor
- Enable loopback test

---

## RS485 Test

- Connect two adapters
- Use Modbus/Serial software
- Verify communication

---

## RS232 Test

- Connect DB9 device
- Open terminal software
- Verify TX/RX communication

---

# 📊 Future Improvements

- [ ] Automatic Direction Control for RS485
- [ ] Isolation Circuit
- [ ] USB Type-C PD Support
- [ ] Metal Enclosure
- [ ] OLED Status Display
- [ ] Baud Rate DIP Switch
- [ ] STM32 Based Smart Version

---

# 🧰 Applications

✔ PLC Communication  
✔ Industrial Automation  
✔ Embedded Debugging  
✔ Serial Protocol Analysis  
✔ Firmware Uploading  
✔ Modbus Communication  
✔ Robotics Projects  
✔ IoT Development

---

# 📸 Screenshots

| Description | Preview |
|------------|---------|
| PCB Front | Add Image |
| PCB Back | Add Image |
| Assembled Board | Add Image |
| Serial Test | Add Image |

---

# 🤝 Contributing

Pull requests are welcome!

If you'd like to improve this project:

1. Fork repository
2. Create feature branch
3. Commit changes
4. Submit PR

---

# 📝 License

This project is licensed under the MIT License.

---

# ❤️ Author

## EmbSysTech Innovations

> Bytes of Innovations

Designed with passion for embedded systems & hardware engineering.

---

# ⭐ Support

If you like this project:

⭐ Star the repository  
🍴 Fork the project  
📢 Share with makers & developers

---

# 📬 Contact

- YouTube: Add Channel Link
- GitHub: Add GitHub Link
- Website: Add Website

---

# 🔥 Project Status

🚧 Currently in Development Phase

PCB Design → Prototype → Testing → Production

---

# 📌 Notes

⚠ RS232 uses voltage levels different from TTL UART.  
⚠ Do not connect RS232 directly to MCU UART pins.  
⚠ Verify power supply before connecting external devices.

---

# 🎯 Goal

Create a reliable, compact, affordable, and professional-grade USB communication tool for makers, students, and engineers.