# HackBot
A robot that is capable of penetration testing

## Requisites
- 1 x Raspberry Pi 3B =>
- 1 x Micro SD card 8Gb =>
- 1 x WiFi USB adapter
- 1 x WebCam
- 1 x Power Bank
- 1 x PCA9685 16 Channel 12 Bit PWM Servo Driver
- 1 x LM2596 Buck Converter, DC-DC step down module
- 12 x MG90S Servo motor
- 4 x Lipo 3.7v battery
- 1 x Toggle Switch
- Some Jumper wires
- Some M3 nuts & bolts

<img src="https://content.instructables.com/FOU/SD48/KID4YXRA/FOUSD48KID4YXRA.jpg?auto=webp&frame=1&width=1024&height=1024&fit=bounds&md=2c2ae9a7eac53b9a71254b45646aac55" align="center" alt="Schematica" title="Schematica">

## Operating System
it is recommended to use a penetration test oriented distro such as [ParrotOS](https://www.parrotsec.org/) or [Kali Linux](https://www.kali.org/) (I used ParrotOS)

- ParrotOS [Download](https://www.parrotsec.org/download/)
- Kali Linux [Download](https://www.kali.org/get-kali/#kali-arm)

## Software
for the web server I used apache2

    sudo apt install apache2
    
and I used shellinabox for the terminal connected to the web interface so I have all full control of the device from the web browser

    sudo apt install shellinabox
