# MICROOVEN - Microwave Oven Project

## Overview

The **MICROOVEN** project is a software implementation of a microwave oven using the **PIC16F877A** microcontroller. It is developed in **MPLAB IDE**, compiled using **XC8**, and simulated in **PICSIMLAB**. This project enables different cooking modes with a user-friendly interface and can be deployed on the **Picgenious** development board.

## Features

This microwave oven project supports multiple operational modes:

- **Power ON Message Screen**: Displays a welcome message when powered on.
- **Micro Mode**: Standard microwave heating mode.
- **Grill Mode**: Grill cooking feature.
- **Convection Mode**: Baking with a fan-assisted heat system.
- **Start Screen**: Indicates that the cooking process is active.
- **Stop Screen**: Displays when cooking is stopped.

## Components Used

### **Hardware**

- **Microcontroller**: PIC16F877A
- **Development Board**: Picgenious
- **Display**: LCD (16x2 or similar, if applicable)
- **Input Interface**: Keypad for mode selection and time input
- **Relays & Drivers**: For controlling power to the heating element
- **Buzzer**: To indicate alerts and cooking completion

### **Software Tools**

- **Host Machine**: Laptop
- **IDE**: MPLAB X IDE
- **Compiler**: XC8 Compiler
- **Simulator**: PICSIMLAB (for testing before hardware implementation)

## Getting Started

### **1. Installation of Software**

Before starting, ensure you have the following installed:

- **MPLAB X IDE** ([Download Here](https://www.microchip.com/mplab/mplab-x-ide))
- **XC8 Compiler** ([Download Here](https://www.microchip.com/mplab/compilers))
- **PICSIMLAB** for software simulation

### **3. Open the Project in MPLAB X IDE**

- Launch **MPLAB X IDE**
- Navigate to **File > Open Project**
- Select the `MICROOVEN` project directory
- Ensure that the **XC8 Compiler** is configured correctly

### **4. Build and Upload to PIC16F877A**

- Click on **Build Project** (or press F11) to compile the source code
- Use a PIC programmer to upload the generated **.hex** file to the **Picgenious** board

### **5. Simulating in PICSIMLAB (Optional)**

If you want to test the project before using real hardware:

- Open **PICSIMLAB**
- Load the compiled **.hex** file
- Simulate the operation to verify expected behavior

## Usage Instructions

1. Power on the system.
2. Select the desired cooking mode using the keypad.
3. Set the cooking time (if applicable).
4. Press **Start** to begin cooking.
5. Press **Stop** at any time to cancel the process.
6. The LCD (if used) will display the active mode and remaining time.

## Project Files

The repository contains the following files:

1. **main.c** – Main program file handling system operations.
2. **main.h** – Configuration settings for the microcontroller.
3. **clcd.c / clcd.h** – LCD control functions.
4. **keypad_matrix.c / keypad_matrix.h** – Code for handling keypad inputs.
5. **microoven.c / microoven.h** – Implementation of different microwave modes.
6. **timer.c / timer.h** – Timer functions for countdown operations.
7. **isr.c ** – Build system for timer.

## Troubleshooting

- **No Display on LCD?** Ensure the connections are correct and the power supply is stable.
- **Program Not Uploading?** Check if the PIC16F877A is properly connected to the programmer.
- **Unexpected Behavior in Simulation?** Ensure that the correct **.hex** file is loaded.

For any questions or suggestions, reach out via GitHub Issues or discussions.

