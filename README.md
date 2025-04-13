# STM32-Development-Board
## Overview

This project is a Printed Circuit Board (PCB) design for a development/evaluation board centered around an STM32 microcontroller. The board is designed to facilitate testing, programming, and experimentation with the STM32, providing a foundation for various applications.

## Project Goals

* Design a versatile development board for STM32 microcontrollers.
* Provide essential interfaces for programming and communication.
* Include a basic output for initial testing and feedback.
* Create a compact and efficient board layout.
* Produce design files for manufacturing and future use.

## Circuit Functionality

The PCB is a development board. It allows a developer to experiment with the STM32 and create various applications.

## Key Components

Here's a breakdown of the main components on the board:

* **U2: STM32 Microcontroller (STM32F411CEU6):**
    * The core of the board.  It's a high-performance, low-power microcontroller that can be programmed to control various functions.
    * It has a wide range of peripherals, including timers, communication interfaces, and analog-to-digital converters.
* **USB Connector (USB):**
    * Provides connectivity to a computer.
    * Functions:
        * Powers the board (5V).
        * Enables programming of the STM32.
        * Facilitates data communication between the STM32 and the computer.
* **SWD Connector (SWD):**
    * Serial Wire Debug port.
    * Used for direct programming and debugging of the STM32 microcontroller.  This is a key interface for development.
* **UART Connector (UART):**
    * Universal Asynchronous Receiver/Transmitter.
    * Enables serial communication with other devices, such as other microcontrollers, sensors, or a computer.  Often used for sending debug messages or exchanging data.
* **SW1: BOOT Button (BOOT):**
    * Controls the boot mode of the STM32.
    * By pressing this button during power-up, the microcontroller can be forced into a specific boot mode, typically used for firmware programming.
* **D1: Red LED (LED):**
    * Provides a visual indication of the board's status.
    * Common uses:
        * Power-on indicator.
        * General-purpose status flag (e.g., indicating the STM32 is running or a specific event has occurred).
* **R1, R2, R3 (Resistors):**
    * Used to limit current.
    * Specifically, R1 limits the current to the USB power input. R2 limits the current for the BOOT button. R3 limits the current to the LED.
* **C1, C2, C3, C4, C5, C6, C7, C8, C9, C10, C11, C12, C13 (Capacitors):**
    * Used for filtering and stabilization.
    * Purpose:
        * Smoothing the power supply to ensure stable operation of the STM32.
        * Filtering out noise from the power supply.
        * Decoupling capacitors are placed close to the STM32 to provide a stable voltage.
* **FB1 (Ferrite Bead):**
    * An electronic component used to suppress high-frequency noise or electromagnetic interference (EMI).

## Project Files

The repository contains the following files:

* `STM32_Dev_Board.kicad_sch`: KiCad schematic file.
* `STM32_Dev_Board.kicad_pcb`: KiCad PCB layout file.
* `STM32_Dev_Board_BOM.csv`: Bill of Materials (BOM) in CSV format.
* `Learnings.md`: A file documenting the learning outcomes and gains from this project.
* `README.md`: This file.


