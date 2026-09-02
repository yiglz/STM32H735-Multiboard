# STM32H735 Multiboard

Custom STM32H7-based embedded hardware platform designed for mixed-signal measurement and high-speed interfacing.

## Overview

This board combines a general-purpose embedded platform (Ethernet, USB HS, CAN-FD, local storage) with a precision analog front-end capable of impedance/frequency-response measurement. The idea was to have something that can act both as a data acquisition node and a small bench instrument on the same board.

## Features

- STM32H735 (Cortex-M7) MCU, 0.65mm pitch BGA
- 128Mbit SDRAM and 128Mbit QSPI NOR Flash, plus microSD for local storage and waveform logging
- 100BASE-T Ethernet (RMII), USB 2.0 HS (ULPI), and CAN-FD interfaces
- 16-bit, 4 MSPS simultaneous-sampling ADC front-end with protected, filtered, differentially-driven inputs
- Onboard DAC-driven excitation path with selectable reference resistors, forming a Bode analyzer / RLC impedance meter for characterizing an unknown DUT
- Dual power input (DC-jack + USB Type-C) with automatic priority switching

## PCB Design

Routed with signal integrity and delay matching in mind, using values that stay within what's standard for essentially every PCB manufacturer(minimum 4mil trace width/spacing, 0.2mm via hole, 0.4mm pad). No via-in-pad, microvia, or buried/blind vias were used.

## Repository Contents

- [Schematic PDF](./Schematic_STM32H735Multiboard.pdf)
- [Gerbers](./GerberFiles)
- [Draftsman](./Draftsman_STM32H735Multiboard.pdf)

## Project Status

- Schematic: Complete
- PCB Design: Complete
- Firmware: Not started yet
