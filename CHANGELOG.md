# Changelog

All notable changes to this project will be documented in this file.

The format follows Keep a Changelog principles.

---

## [0.1.0] - 2026-05-14

### Added

#### Core Hardware

* CH340K USB-to-UART bridge
* USB Type-C interface
* USB ESD protection circuitry
* TX/RX activity indicators
* Power status LED

#### Isolation

* ISO7721 digital isolator
* MEJ1S0505SC isolated DC-DC converter
* MIC5219 3.3V regulator
* Fully isolated target-side UART

#### ESP32 Support

* Dedicated ESP32 programming header
* Auto-programming circuit using RTS/DTR
* EN reset control
* IO0 boot control
* Reset pushbutton
* Boot pushbutton

#### RS485 Interface

* ISL3172E RS485 transceiver
* Selectable 120Ω termination resistor
* Industrial communication support

#### RS232 Interface

* MAX3232 RS232 transceiver
* DB9 serial connector

#### Debug Features

* Dedicated UART debug header
* Clearly labeled connectors
* Color-coded silkscreen markings

### PCB

* Compact PCB layout
* Ground-pour optimization
* Isolation barrier implementation
* Manufacturing-ready design

### Documentation

* Initial project documentation
* Interface descriptions
* Hardware architecture overview

---

## Upcoming

### Planned for v0.2.0

* Prototype validation results
* Communication performance measurements
* Isolation testing report
* RS485 interoperability testing
* ESP32 programming verification
* Manufacturing notes
