# HackBot
A robot that is capable of penetration testing

## Requisites
- 1 x Raspberry Pi 3B =>
- 1 x Micro SD card 8Gb =>
- 1 x WebCam
- 1 x Power Bank
- 1 x PCA9685 16 Channel 12 Bit PWM Servo Driver
- 1 x LM2596 Buck Converter, DC-DC step down module
- 12 x MG90S Servo motor
- 4 x Lipo 3.7v battery
- 1 x Toggle Switch
- Some Jumper wires
- Some M3 nuts & bolts

## Operating System
it is recommended to use a penetration test oriented distro such as [ParrotOS](https://www.parrotsec.org/) or [Kali Linux](https://www.kali.org/) (I used ParrotOS)

- ParrotOS [Download](https://www.parrotsec.org/download/)
- Kali Linux [Download](https://www.kali.org/get-kali/#kali-arm)

## Software

Building & Installation
=======================

You must have cmake installed. You will also probably want to have a development
version of libjpeg installed. I used libjpeg8-dev. e.g.

    sudo apt-get install cmake libjpeg8-dev

If you do not have gcc (and g++ for the opencv plugin) you may need to install those.

    sudo apt-get install gcc g++

Simple compilation
------------------

This will build and install all plugins that can be compiled.

    cd mjpg-streamer-experimental
    make
    sudo make install
    
By default, everything will be compiled in "release" mode. If you wish to compile
with debugging symbols enabled, you can do this:

    cd mjpg-streamer-experimental
    make distclean
    make CMAKE_BUILD_TYPE=Debug
    sudo make install
