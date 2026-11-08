# STM32 Custom Development Board

My first custom STM32 development board, designed using **KiCad** by following the PCB design tutorial from **Phil's Lab**.

The board is based on the **STM32F103C8T6** microcontroller. The main objective of this project was to learn the complete PCB design process, starting from schematic creation and component selection to PCB layout, routing, and preparing manufacturing files.

I also made an improvement to the original tutorial design by bringing the otherwise-unused GPIO pins out to dedicated pin headers, making them accessible for connecting external modules and peripherals.

## Project Overview

This project is my first attempt at designing a custom microcontroller development board rather than relying on a ready-made development module.

The design follows the STM32 hardware design concepts explained in Phil's Lab's tutorial, with an additional focus on making more GPIO pins accessible for general-purpose use.

## Hardware Features

- **Microcontroller:** STM32F103C8T6 (ARM Cortex-M3).
- **USB Interface:** USB Micro-B connector.
- **Power Supply:** 3.3 V power regulation.
- **Clock Circuit:** External high-speed crystal oscillator.
- **Programming and Debugging:** SWD interface.
- **Reset and Boot Configuration:** Dedicated reset and boot circuitry.
- **GPIO Accessibility:** Additional pin headers to expose otherwise-unused GPIO pins.
- **PCB:** Custom-designed two-layer PCB.

## My Improvements
### GPIO Expansion Through Pin Headers
The original tutorial design did not expose all available STM32 GPIO pins. I modified the PCB by routing the otherwise-unused GPIO pins to dedicated pin headers.

This allows easy access to additional GPIOs for connecting sensors, displays, communication modules (UART, SPI, I2C), and other external peripherals, making the board more flexible for future projects and prototyping.

## Design and Development Process

The board was designed using the following workflow:

1. **Schematic Design:** Created the STM32-based circuit schematic in KiCad.
2. **Component Selection:** Selected the required components, connectors, and footprints.
3. **PCB Layout:** Arranged the components while considering signal routing and board dimensions.
4. **PCB Routing:** Routed the connections across the two copper layers.
5. **GPIO Expansion:** Added pin headers to expose the otherwise-unused GPIO pins.
6. **Design Verification:** Checked the schematic and PCB using KiCad's Electrical Rules Checker (ERC) and Design Rules Checker (DRC).
7. **3D Inspection:** Used KiCad's 3D viewer to inspect the board layout.

## Tools Used

- **KiCad** – Schematic capture and PCB design.
- **STM32CubeIDE** – STM32 microcontroller pinout and peripheral reference.
- **Phil's Lab Tutorial** – Reference for the STM32 hardware and PCB design process.

## Project Images

Add your own board images below:

### 3D PCB View

<img width="1003" height="777" alt="image" src="https://github.com/user-attachments/assets/3e046da7-37d9-48c0-87ed-16af264071d7" />


### PCB Layout

<img width="1042" height="767" alt="image" src="https://github.com/user-attachments/assets/89371302-6cb0-43e3-8b66-3985f8531ed1" />


### Schematic
<img width="1106" height="766" alt="image" src="https://github.com/user-attachments/assets/10552613-4e4f-4a4e-a5f0-75802422dd52" />


## Learning Outcomes

Through this project, I gained practical experience in:

- Designing a custom STM32-based development board.
- Understanding the basic hardware requirements of an STM32 microcontroller.
- Creating schematics and assigning component footprints in KiCad.
- PCB component placement and signal routing.
- Understanding power, clock, USB, and SWD connections.
- Exposing GPIO pins for external hardware interfacing.
- Performing ERC and DRC checks.
- Preparing PCB manufacturing files.

## Reference

This project was developed by following the tutorial by **Phil's Lab**:

[STM32 Hardware Design and PCB Design with KiCad – Phil's Lab](https://www.youtube.com/watch?v=aVUqaB0IMh4)

The original tutorial served as the foundation for the board design. The GPIO pin-header expansion was my own modification to improve the accessibility and usability of the board.

---

**Note:** This is my first custom development board project and an important step in learning embedded hardware and PCB design.
