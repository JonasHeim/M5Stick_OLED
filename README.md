Work in progress

# M5Stick OLED

[![Build Status](http://ci.jonasheim.de/buildStatus/icon?job=M5Stick_OLED)](http://ci.jonasheim.de/job/M5Stick_OLED)

This is a minimal OLED driver example running on an ESP32; more precise on a [M5Stick](https://docs.m5stack.com/#/en/core/m5stick).

The application is based on the ESP32 [ESP-IDF](https://github.com/espressif/esp-idf) SDK by Espressif.

## OLED
The M5Stick integrates an 1.3" OLED with a resolution of 64x128 Pixels that is interfaced using a [SH1107 Dot Matrix Controller](https://www.displayfuture.com/Display/datasheet/controller/SH1107.pdf).

The OLED controller is connected via 3-Wire SPI to the ESP32 with the following Pin assignments:

| ESP32 | Signal |
| ----------- | ----------- |
| GPIO14 | Chip Select (CS) |
| GPIO33 | Reset | 
| GPIO27 | D/C | 
| GPIO18 | SCLK (D0) | 
| GPIO23 | MOSI (D1) | 


Reference to M5Stick [schematic](https://github.com/m5stack/M5-Schematic/blob/master/Core/m5stick/EspCore.pdf).
