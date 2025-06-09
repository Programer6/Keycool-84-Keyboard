# Keycool-84-Keyboard

# STM32-Ortho6x16 - A Custom Mechanical Keyboard

## Table of Contents
1.  [Introduction](#introduction)
2.  [My Journey](#my-journey)
3.  [Features](#features)
4.  [Hardware Details](#hardware-details)
    *   [Microcontroller](#microcontroller)
    *   [Key Matrix](#key-matrix)
    *   [RGB Lighting](#rgb-lighting)
    *   [OLED Display](#oled-display)
    *   [Connectivity](#connectivity)
    *   [Protection & Power](#protection--power)
5.  [Firmware (QMK)](#firmware-qmk)
    *   [Keymap](#keymap)
    *   [Compiling](#compiling)
    *   [Flashing](#flashing)
6.  [Bill of Materials (Key Components)](#bill-of-materials-key-components)
7.  [Future Ideas / To-Do](#future-ideas--to-do)
8.  [Acknowledgements](#acknowledgements)



## Introduction

The STM32-Ortho6x16 is a custom-designed and hand-built mechanical keyboard featuring a 6-row by 16-column matrix, per-key addressable RGB LEDs, and an OLED display for status information. It's powered by an STM32F072 microcontroller and runs custom QMK firmware. This project was born out of a desire to learn PCB design keyboards design.

## My journey

## Features

*   **Custom 6x16 Key Matrix:** (Up to 96 keys) Configurable layout via QMK.
*   **STM32F072CBT6 Microcontroller:** Powerful Arm Cortex-M0 MCU.
*   **QMK Firmware:** Fully programmable and customizable.
*   **Per-Key Addressable RGB Lighting:** WS2812B LEDs 12 LEDs in total.
*   **SSD1306 OLED Display (128x32):** Shows current layer, lock key status, and RGB status.(Can be customized to you liking)
*   **USB-C Connectivity:** Modern and robust connector.
*   **Hardware Reset Button & Boot0 Pin Access:** For easy firmware flashing.
*   **ESD Protection:** On USB data lines (U2 - PRTR5V0U2X).
*   **Overcurrent Protection:** 500mA fuse (F1) on VBUS.
*   **Level Shifter (TXB0101):** For shifting 3.3V RGB data signal to 5V for WS2812B LEDs.

## Hardware Details

### Microcontroller
*   **MCU:** STM32F072CBT6 (LQFP48 package)
*   **Core:** Arm Cortex-M0

### Key Matrix
*   **Layout:** 6 Rows x 16 Columns
*   **Row Pins (STM32):** PA0 (row0), PA1 (row1), PA2 (row2), PA3 (row3), PA4 (row4), PA5 (row5)
*   **Column Pins (STM32):**
    *   PA7 (col0), PA6 (col1), PA9 (col2), PA10 (col3), PA15 (col4),
    *   PB0 (col5), PB1 (col6), PB2 (col7), PB3 (col8), PB4 (col9), PB5 (col10), PB6 (col11), PB7 (col12),
    *   PC13 (col13), PC14 (col14), PC15 (col15)
*   **Diode Direction:** Column to Row (COL2ROW)

### RGB Lighting



### OLED Display



### Connectivity



## Firmware (QMK)

