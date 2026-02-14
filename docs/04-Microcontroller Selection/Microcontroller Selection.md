---
title: Microcontroller Selection
---

## Subsystem Responsibilities

My subsystem will be responsible for detecting the temperature of water and then conveying the to our control board being operated by Adrian. I will be using a TC74A4-3.3VCTTR temperature sensor that has an operating current of 200 mA, and since I will be using the PIC18F47K42 my subsystem will only need 3.3V and around 250 mA of current to operate safely which allows the rest of my team more flexibility with their designs. We will be communicating via UART and I will be sending an 8-bit digital word to Adrian. 

## Temperature Sensor MPLabX Configuration 

![Temperature Sensor Config](TempConfig.png)

## Pin Functions

RC3 is my TX and will be sending the 8-Bit data to Adrians control board so he can use it to display the information to the user. I will be using RB0 as a GPIO to simply have a debugging LED so I can troubleshoot my code. Finally we have RB6 and RB7 which are my serial clock/data and are going to be connected to their respective pins on the temperature sensor and will be responsible for reading the data and converting into an 8-Bit digital word that I will then be able to send to my teammates via UART.

## Final Selection

I have decided to proceed with the PIC18F47K42 because of it's minimal current and voltage operating ranges, because my responsibility will only be to send data to Adrian it made sense to go with the PIC as opposed to and ESP32 for example because my subsystem has no use for Wifi/bluetooth. The pic also has the appropriate SCL and SDA pins needed to operate my temperature sensor while leaving many other pins open for the rest of my team to use as some of their systems require more pins because of their communication types. In addition to this the rest of our team is using the ESP32 and per project requirements we needed at least one person to use a PIC and my subsystem made the most sense for that.