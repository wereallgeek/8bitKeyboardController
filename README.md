# 8bitKeyboardController - a retro keyboard matrix controller PCB
# C16/C64 QMK/VIAL USB & PS/2 Keyboard controller

## Purpose

PCB to interface vintage 8bit keyboard with a Raspberry Pi pico to run as a Keyboard controller.

Meant to take a C16 or C64 keyboard matrix (different firmware) and map it on the controller, to enable USB -or- PS/2 connectivity (selectable by jumper)

The device is VIAL compliant and can be fully remapped at https://vial.rocks/


## Hardware

This PCB has been developped on KiCad v10 

It has two 20-pin connectors, only one to be used depending on firmware. the C16 & C64 matrix are not compatible.

<p align="center">
  <img src="https://raw.githubusercontent.com/wereallgeek/8bitKeyboardController/main/images/3dpcb.png">
</p>

The hardware has provisions for keyboard leds but they currently are non-functionnal when in PS/2 mode. Likely related to how the PS/2 protocol is bit-banged, causing bidirectional communication to fail and LED status to not update. This may be resolved in the future.

There is also provision for an added capslock switch - meant mainly for C64 while using a mechboard.


## Firmware

Compatible QMK/Vial firmware is present on my fork of Vial

see https://github.com/wereallgeek/vial-qmk

precompiled variants are available there

https://github.com/wereallgeek/vial-qmk/tree/vial/binaries


## Copyright (C) 2026 Marsupial (wereallgeeks.wordpress.com) 


This PCB Design is free hardware: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation version 3,see [license](https://github.com/wereallgeek/8bitKeyboardController?tab=License-1-ov-file), as long as PCB attribution markings and silkscreen remains present on the final product.

Commercial profitability is strictly prohibited

This design is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE,  or FUNCTIONALITY. 
See the [License](https://github.com/wereallgeek/8bitKeyboardController?tab=License-1-ov-file) for more details.

