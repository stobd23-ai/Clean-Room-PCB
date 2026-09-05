# Clean-Room-PCB - Clean Room Monitoring System Redesign
Redesigned and implemented the hardware architecture of an ESP32-based clean room monitoring system, developing the schematic and custom PCB in Fusion 360 Electronics. Integrated sensor interfaces, power management, USB-to-UART programming, data logging, and IoT connectivity. Debugged and optimised the embedded firmware and implemented remote monitoring and notification functionality.

## Features

- **Multi-Sensor Monitoring:** Integrates temperature, humidity, pressure, oxygen, and particle sensors with an ESP32-based control system.
- **Real-Time Data Logging & Display:** Displays environmental readings on an LCD while storing measurements on an SD card for long-term monitoring and analysis.
- **Reliable Power & Embedded Design:** Features a custom PCB with regulated 3.3V/5V power, rechargeable battery backup, protection circuitry, and ESP32 auto-programming support.
- **Automated Cleanliness Detection:** Compares sensor readings against predefined acceptable limits and determines whether the environment is Clean or Not Clean.
- **USB Programming Interface:** Uses a CP2102 USB-to-UART interface for programming and communication with the ESP32.
- **Automatic ESP32 Programming:** Includes BOOT and RESET circuitry to simplify uploading firmware to the ESP32.
- **Remote IoT Monitoring:** Connects the system to the Blynk IoT platform so environmental conditions can be monitored remotely.

## Tech Stack

- **Language:** C++ (in Arduino)

- **Frameworks/Libraries:**

ESP32 HardwareSerial — Serial communication with the PMS5003 particle sensor
WiFi — ESP32 Wi-Fi connectivity
Blynk — IoT connectivity, remote monitoring, and notifications
DHT sensor library — Interface with the DHT22 temperature and humidity sensor
Wire — I²C communication for the oxygen sensor
LiquidCrystal — Control of the RG2004A parallel LCD
SPI — SPI communication for the SD card
SD — SD card data logging

- **Database/Tools:** Fusion360, Arduino, VSCode extension

## License

Educational Use Only License

Copyright © 2026 [Sonam Tobden]. All Rights Reserved.

This project is provided for educational and personal learning purposes only.

Permission is granted to view and study the source code, documentation, schematics, and other materials included in this repository for educational purposes.

The following are NOT permitted without explicit written permission from the copyright holder:

Copying or reproducing this project or substantial portions of it.
Modifying, adapting, or creating derivative works from this project.
Redistributing, republishing, or uploading the project or its contents elsewhere.
Using this project or its contents in another project, product, or publication.
Using this project for commercial purposes.
Claiming any part of this project as your own work.

If you wish to use, modify, reproduce, or redistribute any part of this project beyond personal educational study, you must obtain prior written permission from the copyright holder.

By accessing this repository, you agree to these terms.

This is not an open-source license. All rights are reserved except for the limited educational viewing permission stated above.
