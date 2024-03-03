**Project Name:** FreeRTOS_Voltmeter**

## Overview
The Voltmeter Application is designed to measure and display voltage readings using microcontroller-based hardware and a graphical user interface (GUI) for user interaction.

**Description:**

This project is based on the STM32 Nucleo-64 development board and utilizes the FreeRTOS operating system to implement a voltmeter application. It leverages the ILI9341 LCD for displaying the voltage readings and includes functionalities like:

* **ADC (Analog-to-Digital Converter) integration:** Measures the analog voltage input.
* **TouchGFX integration:** Provides a graphical user interface for the voltmeter readings.
* **Semaphores:** Ensure proper synchronization between tasks accessing shared resources (e.g., ADC data).

## Features
- Measurement of voltage levels
- Graphical display of voltage readings
- User-friendly interface for interaction
- Real-time updates of voltage measurements

**Hardware Requirements:**

* STM32 Nucleo-64 development board
* ILI9341 LCD display
* Analog-to-digital converter (ADC)
* Communication interfaces (e.g., SPI, I2C)
* Voltage sensing circuitry (e.g., voltage divider)
* Additional components for voltage measurement circuit (resistor, voltage regulator, etc.)

**Software Requirements:**

* STM32CubeMX
* FreeRTOS
* TouchGFX (optional, for graphical UI)

## Software Components
- Microcontroller firmware written in C
- TouchGFX for GUI development
- Peripheral drivers (ADC, DMA, SPI, I2C)
- Real-time operating system (RTOS) for task scheduling (e.g., FreeRTOS)
- Libraries for hardware abstraction and communication protocols

  ## Project Structure
- **Src**: Contains source code files for the microcontroller firmware.
- **Inc**: Header files for the firmware.
- **TouchGFX**: TouchGFX project files for the graphical interface.
- **Drivers**: Peripheral drivers provided by the microcontroller manufacturer.
- **Middlewares**: Middleware components used in the project (e.g., FreeRTOS).

**License:**

Apache License 2.0

**How to Use:**

1. Download the project files, including the main.c file and any additional source files and header files.
2. Import the project into your IDE (e.g., STM32CubeIDE).
3. Configure the project settings according to your hardware setup, including clock configuration, pin assignments, and ADC parameters.
4. Build and program the project onto your development board.
5. Connect the voltage source to the designated input pin.
6. (Optional) If using TouchGFX, build and deploy the graphical user interface to the target device.

## Usage 
1. Power on the device.
2. Use the touchscreen interface to navigate through the options and view voltage readings.
3. Calibrate the device if necessary.
4. Obtain voltage measurements from the display.

## Future Improvements
- Implement additional features such as data logging and graph plotting.
- Enhance user interface design for better user experience.
- Optimize power consumption for extended battery life.
- Add support for multiple voltage ranges and measurement modes.

**Note:**

This is a basic overview of the project. Refer to the specific code implementation and hardware schematics for detailed instructions and modifications.
