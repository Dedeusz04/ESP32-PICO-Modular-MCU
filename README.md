# ESP32-PICO Modular MCU

A modular hardware design based on the ESP32-PICO microcontroller, split into separate, specialized boards for the processor, power supply, and clock management to ensure high flexibility and easier troubleshooting in embedded development.

## Key Features
- **Modular Architecture**: Core system functionality is divided into distinct, easily interchangeable boards.
- **Processor Module** (`modul_procesora`): Houses the ESP32-PICO core, providing native Wi-Fi/Bluetooth capabilities and GPIO breakouts.
- **Power Supply Module** (`modul_zasilania`): Dedicated hardware for voltage regulation and stable power distribution to all components.
- **Clock Module** (`modul_zegara`): Handles precise clock generation and timing logic.
- **Custom Component Library**: Includes a comprehensive custom Autodesk EAGLE library (`proj_biblioteka.lbr`) with all necessary footprints and symbols used.

For a detailed description of the design, schematic choices, and PCB layouts, refer to the final project report included in this repository: [raport_koncowy_tem1 2 (1).pdf](raport_koncowy_tem1%202%20%281%29.pdf).

## Modules Overview
| Module | Schematic File | Board File | Description |
|---|---|---|---|
| **Processor Module** | `modul_procesora.sch` | `modul_procesora.brd` | Core ESP32-PICO system |
| **Power Supply** | `modul_zasilania.sch` | `modul_zasilania.brd` | Voltage regulation and power management |
| **Clock Module** | `modul_zegara.sch` | `modul_zegara.brd` | Precise timers and RTC |

## Usage
The hardware designs are provided as Autodesk EAGLE files.
1. Clone or download this repository.
2. Open Autodesk EAGLE and ensure `proj_biblioteka.lbr` is added to your active libraries.
3. Open the `.sch` and `.brd` files to view, modify, or manufacture the schematics and PCB designs.

*Note: To run firmware on the Processor Module, you can use PlatformIO or the standard ESP-IDF / Arduino IDE configured for the ESP32-PICO-D4.*

## Contributors
- **Bartosz Kępa**
- **Jan Jamro**
- **Aleksandra Kuś**
