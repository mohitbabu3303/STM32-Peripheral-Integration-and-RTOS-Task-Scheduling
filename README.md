# STM32 Peripheral Integration with FreeRTOS Task Scheduling

## Overview
This project demonstrates the integration of multiple peripherals on an STM32 microcontroller with multitasking using FreeRTOS. It includes real-time sensor data acquisition, processing, and communication, highlighting efficient peripheral use, DMA, and interrupt-driven design.

The system architecture is modular, with each functional unit implemented as a separate FreeRTOS task, ensuring scalable and maintainable embedded development.

---

## Features
- STM32 microcontroller-based real-time multitasking system
- Peripheral integration:
  - UART for PC communication
  - I²C/SPI sensors (temperature, humidity, ultrasonic)
  - GPIO for buttons and LEDs
  - DMA for efficient data transfer
- FreeRTOS task scheduling with queues, semaphores, and mutexes
- Watchdog timer for system reliability
- Modular and scalable architecture for easy extension
- Debugging support with STM32CubeIDE, UART logs, and FreeRTOS trace

---

## Hardware Requirements
- STM32 Board (F4 Discovery / Nucleo or equivalent)
- Temperature & Humidity Sensor (DHT11/DHT22 or I²C-based)
- Ultrasonic Sensor (HC-SR04)
- LEDs & Push Buttons
- USB-UART converter (optional)
- ST-Link debugger
- Breadboard and jumper wires

---

## Software Requirements
- STM32CubeIDE
- STM32CubeMX
- FreeRTOS
- Optional: Keil µVision, Proteus, MATLAB/Simulink, STM32CubeMonitor

---

## Project Structure
/STM32_FreeRTOS_Project
│
├── Core
│ ├── Inc # Header files
│ └── Src # Source files (tasks, peripheral drivers)
│
├── Drivers
│ ├── CMSIS
│ └── STM32 HAL
│
├── FreeRTOS
│ └── Source # RTOS kernel files
│
├── .gitignore
├── README.md
└── STM32CubeIDE project files
