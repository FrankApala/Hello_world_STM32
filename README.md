# Bare-Metal LED Blink for NUCLEO-F103RB

This repository contains a simple "Hello World" example targeting the STM32F103RB NUCLEO board. The code was originally generated with STM32CubeIDE but all HAL initialization calls have been commented out so that only direct register accesses remain. It demonstrates how to toggle an on-board LED without relying on the HAL library.

## Project Overview
- Enable the GPIOA clock
- Configure **PA8** as a push‑pull output
- Toggle PA8 in a software loop to blink an LED

The `SystemClock_Config` function is retained as an empty stub to highlight that the HAL-based clock setup is unused. The rest of the CubeIDE framework files are kept for reference but are not required for this bare‑metal demo.

## Requirements
- NUCLEO‑F103RB board
- A GNU Arm toolchain (or STM32CubeIDE) with `make`


## License
The CMSIS components are licensed under Apache‑2.0. HAL drivers are BSD‑3‑Clause. See `Drivers/*/LICENSE.txt` for the full texts.
