ATmega328P + BME280 Sensor Breakout Board

📖 Project Overview

This project is a custom-designed microcontroller board based on the ATmega328P, integrated with a BME280 environmental sensor (temperature, humidity, pressure) using the I²C protocol.

The board includes:

On-board clock (crystal oscillator)
Proper power decoupling
ISP programming interface
Clean ERC & DRC-verified PCB layout
3D-validated mechanical design

The goal of this project was to design a production-ready embedded hardware board, following industry best practices.

🧩 Features

ATmega328P (DIP package) microcontroller
BME280 sensor (I²C mode)
External crystal oscillator with load capacitors
Proper AVCC, VCC, and AREF handling
ISP header for programming (AVR-ISP)
Fully ERC & DRC clean design
Compact, single-board solution

⚙️ Hardware Specifications
Component	Description
MCU	ATmega328P
Sensor	Bosch BME280
Interface	I²C
Clock	External crystal
Programming	AVR ISP (SPI)
Supply Voltage	5V
PCB Layers	2-layer

🔌 Pin Configuration (Key Connections)

ATmega328P
VCC / AVCC → 5V (with decoupling capacitors)
AREF → 100nF capacitor to GND
XTAL1 / XTAL2 → External crystal + 22pF caps
RESET → Pull-up resistor (10kΩ)
SPI Pins → Connected to ISP header

BME280 (I²C Mode)

SDI (SDA) → MCU SDA
SCK (SCL) → MCU SCL
CSB → Pulled HIGH (I²C selection)
SDO → GND (I²C address = 0x76)

🛠️ Design Workflow

Schematic design with ERC validation
Footprint assignment & verification
PCB placement with routing optimization
Manual routing (no autorouter)
DRC clean check
3D view validation

🧪 Design Checks

✅ ERC: Clean
✅ DRC: Clean
✅ No unconnected nets
✅ Silkscreen overlap resolved

📷 Project Media

Include the following in your GitHub repo:

📄 Schematic PDF
🧠 PCB layout screenshots
🧊 3D render images
🗂 KiCad project files

🚀 Future Improvements

Ground plane pour for EMI reduction
Test pads for debugging
USB-to-UART onboard
Enclosure-ready board outline

🧑‍💻 Tools Used

KiCad (Schematic, PCB, 3D Viewer)
AVR Architecture
I²C Protocol

📜 License

This project is open-source and intended for learning and demonstration purposes.
