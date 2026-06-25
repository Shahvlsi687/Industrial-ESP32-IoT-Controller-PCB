# Industrial ESP32 IoT Controller PCB

A production-ready IoT controller board designed in KiCad. It pairs an ESP32-WROOM-32 MCU with an I2C OLED display interface, supported by a localized low-noise 3.3V power distribution network.

### 🛠️ Hardware Subsystems
* **Processing Core:** ESP32-WROOM-32 module managing wireless communication stacks.
* **Power Regulation:** LM1117 3.3V linear regulator in an SMD SOT-223 package.
* **Power Integrity:** Close-coupled 0805 decoupling loops near VCC pins to prevent transmission brownouts.
* **Peripherals:** 4-pin I2C OLED header (`J2`) with dedicated hardware pull-up resistors (`R1`, `R2`).

### 📐 Engineering Design Choices
* **RF Isolation:** Enforced a copper-free Keep-Out zone around the PCB trace antenna to preserve signal integrity.
* **Signal Quality:** Clean 45-degree trace layout geometry to minimize impedance discontinuities.
* **Fabrication Outputs:** Verified layout with zero Design Rule Check (DRC) violations. 

### 📁 Repository Structure
* `Industrial-ESP32-IoT-Controller-PCB.kicad_pcb`: Core physical board routing file.
* `Gerber_Outputs.zip`: Production-ready copper, mask, silkscreen, and CNC drill data.
* `screenshots/`: 3D isometric simulation renders of the final board.
