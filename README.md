# Timer_Capture_Compare

## Overview

## Overview

This project demonstrates using a timer update event to trigger DMA transfers for LED control and timer input capture to measure the signal's period. Users can connect an LED signal with a frequency ranging from 10 Hz to 300 Hz to PA6 to measure and display its frequency.

## Hardware

- STM32 Nucleo-F446RE development board
- USB connection to PC

## Software and Tools

- STM32CubeIDE
- STM32CubeMX
- STM32 HAL
- C programming language

## Features

- TIM1 is configured to generate update events that trigger DMA transfers to control the blinking of LED2 (PA5).
- TIM3 is configured in input capture mode to measure the frequency of an external signal connected to PA6.
- UART communication is used to display the measured frequency on a PC terminal.

## Project Structure

- `Core/Inc/` — application header files
- `Core/Src/` — application source files
- `Drivers/` — STM32 HAL and CMSIS dependencies
- `.ioc` — STM32CubeMX configuration file
