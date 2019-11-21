# RetroDuino

![](https://github.com/a-wai/retroduino/blob/master/cpu_board.png)

The RetroDuino is an attempt at designing and building an 8-bit microcomputer,
using a 6502 processor, and offering a number of I/O options, as commonly found
on Arduino boards.

## Features

This SBC (Single Board Computer) provides a UART interface, an I2C bus and 24
GPIOs.

It includes 31kB of SRAM, 32kB of flash memory (mounted on a ZIF socket for
easier programming), and runs at 8MHz.

## Internals

The RetroDuino includes:

- 1 65C02 processsor w/ 8MHz oscillator
- 1 GAL22V10 for address decoding logic
- 1 AS6C62256 32kB SRAM
- 1 SST39SF010/020/040 flash memory, of which only 32kB is used
- 1 SCC2691 UART controller
- 1 PCF8584 I2C controller
- 1 82C55A peripheral interface providing 24 GPIO lines

It can be powered using a 7-24V DC power supply.

## Current status

This project is still in its infancy: hardware design is complete, but not
tested yet. The next steps are:

[] program and test the GAL logic
[] prototype a flash programmer (probably using a STM32 board)
[] build the board
[] write the software

## Why?

Why go through so much pain, when hundreds of microcontroller boards are
widely available and so cheap? Because... Well, it's fun!

And as a positive side effect, this is a good way to learn a lot about the
internals of modern microcontrollers, or computers in general.

### Copyright

Copyright 2019, Arnaud Ferraris.

This documentation describes Open Hardware and is licensed under the
CERN OHL v.1.2.

You may redistribute and modify this documentation under the terms of the
[CERN OHL v.1.2](http://ohwr.org/cernohl). This documentation is distributed
WITHOUT ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING OF MERCHANTABILITY,
SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE.

Please see the CERN OHL v.1.2 for applicable conditions.
