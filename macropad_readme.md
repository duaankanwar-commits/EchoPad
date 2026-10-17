# Pico Web-Configurable Macropad

A custom, wired USB HID macropad powered by a Raspberry Pi Pico running CircuitPython. Built for clean and straightforward daily use, it offers full plug-and-play functionality without needing any background scripts on your PC. It features custom 3D-printed keycaps and a web-based configuration tool.

## Overview & Key Features

* **Native USB HID:** Acts as a standard USB keyboard directly at the hardware level. Just plug it in and use it—no drivers or background desktop scripts required.
* **Web Configurator:** A lightweight HTML interface that lets you customize keymaps, shortcuts, and macros easily.
* **CircuitPython Powered:** Simple and easy-to-maintain `code.py` script handling all input logic.
* **Compact Build:** Powered by a Raspberry Pi Pico with swappable, custom 3D-printed red keycaps, trimmed down specifically for utility without excess bulk.

## Hardware Specifications

* Microcontroller: Raspberry Pi Pico
* Firmware: CircuitPython
* Interface: Wired USB (Native HID Keyboard)
* Keycaps: Custom 3D-printed red keycaps (replaceable)

## Repository Structure

```
├── code.py              # Main CircuitPython script
├── lib/                 # Adafruit HID libraries
├── configurator/        # Web configurator interface files
└── README.md            # Documentation
```

## Setup Instructions

### 1. Hardware Assembly
1. Wire mechanical switches to the designated GPIO pins on the Pi Pico.
2. Mount switches into your enclosure and attach the 3D-printed keycaps.

### 2. Microcontroller Setup
1. Flash CircuitPython to the Raspberry Pi Pico.
2. Drag the `adafruit_hid` library folder into the `lib` directory on the Pico.
3. Copy `code.py` to the root folder of the drive.

### 3. Key Configuration
1. Open `configurator/index.html` in any web browser.
2. Define your desired macro mappings.
3. Save or export the configuration file onto the Pico.

## Development Progress & Future Plans

- [x] Initial wiring and layout setup
- [x] Switch from ESP32 to Pi Pico for reliable native HID
- [x] Build working HTML macro configurator
- [x] Print custom red keycaps
- [ ] Host configurator on a permanent domain
- [ ] Design and order a custom PCB for the next revision

## Acknowledgments

Thanks to the Forge community and everyone who provided feedback and advice during the build process.