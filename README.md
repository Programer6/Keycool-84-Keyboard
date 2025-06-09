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
*   **Per-Key Addressable RGB Lighting:** WS2812B LEDs for vibrant lighting effects. The schematic shows D85-D96 (12 LEDs visible).
*   **SSD1306 OLED Display (128x32):** Shows current layer, lock key status, and RGB status.
*   **USB-C Connectivity:** Modern and robust connector.
*   **Hardware Reset Button & Boot0 Pin Access:** For easy firmware flashing.
*   **ESD Protection:** On USB data lines (U2 - PRTR5V0U2X).
*   **Overcurrent Protection:** 500mA fuse (F1) on VBUS.
*   **Level Shifter (TXB0101):** For shifting 3.3V RGB data signal to 5V for WS2812B LEDs.
