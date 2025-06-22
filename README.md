# SmartCoin

## Overview

The **SmartCoin** is an ultra-compact, high-tech device designed to showcase advanced electronics miniaturization and integration. Fitting within the dimensions of a coin, it combines cutting-edge connectivity, environmental sensing, and intuitive user feedback in an incredibly small form factor. This project serves as a comprehensive demonstration of expertise in Altium Designer for complex PCB layout, power management, and component selection for highly constrained designs.

At its core, the **Insight SiP ISP3080-UX module** is a standout feature. With integrated BLE and dual-band (5 and 9) UWB antennas offering global coverage with a single device, the ISP3080 is perfectly suited for **Real-Time Location Systems (RTLS), security bubble applications, access control, and highly accurate indoor positioning.** This module's ability to combine precise UWB ranging with versatile BLE communication is fundamental to the SmartCoin's advanced capabilities.

<img src="Images/SmartCoin (1).png" width="400">
<img src="Images/SmartCoin (2).png" width="400">
<img src="Images/SmartCoin (3).png" width="400">

## Key Features & Capabilities

* **Ultra-Wide Band (UWB) & Bluetooth Low Energy (BLE) Connectivity:** Powered by the **Insight SiP ISP3080-UX module**, the SmartCoin offers high-precision indoor positioning (UWB) and versatile short-range communication (BLE 5.1). This enables applications such as real-time location tracking, secure access control, and low-power data exchange.
* **Comprehensive Environmental Sensing:** Integrates the **Bosch Sensortec BME690 4-in-1 sensor** for real-time measurement of:
    * **Gas Composition:** AI-enhanced detection of Volatile Organic Compounds (VOCs), Volatile Sulfur Compounds (VSCs), Carbon Monoxide (CO), and Hydrogen (H2).
    * **Humidity**
    * **Temperature**
    * **Air Pressure**
    * *I2C Address: 0x76*
* **Ultra-Low Energy Data Storage:** Features the **Renesas AT25EU0161A 16 Mbit Ultra-Low Energy Serial Flash Memory** for robust and power-efficient data logging and firmware storage.
* **Compact Power Management:** Utilizes the **nPM2100 Power Management IC (PMIC)** for efficient power delivery, battery charging, and optimal system voltage regulation. This PMIC is critical for maximizing the operational life from the small battery.
* **Flexible Charging & Connectivity:** Equipped with a **Micro-USB-B port** for convenient battery charging and potential data interface.
* **Audible Feedback:** Incorporates an **80 dB CUI Devices CMT-0503-03-SMT-TR Piezo Buzzer** for clear audible alerts and notifications.
    * *Controlled via GPIO Pin P0.05*
* **Intuitive Visual Feedback:**
    * **RGB LED:** A multi-color LED providing customizable visual indicators for status, alerts, or mode.
        * *Controlled via an I2C RGB Driver (I2C Address: 0x30)*
    * **POWER LED:** A dedicated LED to indicate power status.
* **Debug & Development Ready:** Includes a **TC2050-IDC 10-pin SWD (Serial Wire Debug) port** for seamless firmware development, debugging, and programming.
* **User Control:** A **side press push button** provides a physical interface for reset control or user-defined actions.
* **Compact Power Source:** Powered by a **CR2032 coin cell battery**, chosen for its balance of energy density and compact form factor.
* **Miniaturized Form Factor:** The entire PCB is custom-designed to match the **exact size and circular shape of a 2 Euro coin**, demonstrating extreme component density and intricate routing capabilities.

## Technical Highlights

* **Altium Designer Mastery:** This project extensively utilizes Altium Designer for:
    * **Complex Schematic Capture:** Managing multiple ICs, power rails, and interfaces within a dense system.
    * **High-Density PCB Layout:** Expert component placement and multi-layer routing to achieve the coin-sized form factor while respecting RF constraints (UWB antenna keep-out).
    * **Power Integrity:** Careful design of power distribution networks (PDN) for stable operation of sensitive RF and sensor components.
    * **Signal Integrity:** Optimized routing for high-speed interfaces like SPI (Flash) and I2C (BME690, RGB Driver), and differential pair routing for USB.
* **Low-Power Design Philosophy:** Every component selected and every design decision made emphasizes ultra-low power consumption to maximize battery life, crucial for a device powered by a CR2032.
* **Multi-Sensor Integration:** Seamless integration of UWB, BLE, and a 4-in-1 environmental sensor into a cohesive system.
* **Robust Mechanical Design:** Consideration for component robustness, connector stability (Micro-USB), and physical accessibility of the button and debug port within the miniature footprint.

## Future Possibilities

The SmartCoin platform provides a versatile foundation for various applications, including:
* Personal air quality monitoring.
* Asset tracking and inventory management.
* Context-aware smart home devices.
* Wearable technology and personal safety alerts.
* Educational platform for advanced embedded systems.
