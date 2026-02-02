---
title: Module's Requirements
---

## Module Requirements
My responsibility for this project is to use a temperature sensor that will detect the water's temperature in celsius and will be displayed to the user on the OLED screen implemented in our Human Machine Interface(HMI)

| **Requirement Description** | **Measure of<br> Threshold** | **Target<br>Measure** |**Stretch<br>Requirement<br>(Y-N)**|
|-----------------------------| ----------------- | ----------------- | :-----: |
| Surface mounted, 3.3V switching power regulator | 3.2 Volts | 3.3 Volts | No |
| Surface mounted microcontroller | 1 PIC or ESP | 8-bit PIC | No |
| Wireless Communication | Able to send or receive a Wi-Fi data | Send and receive Wi-Fi Data to MQTT | Yes |
|Shared power rail | 3.2 volts | 3.3 volts | **NO** |
|I2C Communication Interface | I2C Communication | I2C with selectable address | **NO** |
|Shared power rail | 3.2 volts | 3.3 volts | **NO** |
|Temperature Sensor | Celsius | ± 1 celsius accuracy | **NO** |
|Data transmission to MCU and HMI | Serial UART at 9600 baud | I2C AND wireless transmission | **NO** |