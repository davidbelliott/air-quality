# IoT Air Quality Monitor Board

![3D render of the board](doc/fig/board-3d.png)

## Overview

This is an ESP32-based IoT air quality monitor board. It features a BME280 for temperature, pressure, and humidity readings, and a CCS811 for CO<sub>2</sub> and TVOX readings. The BME280 temperature reading is also used to calibrate the CCS811. The board connects to the internet, and a web application communicating with the device using a RESTful API provides graphs of all measured quantities over time. The device includes a piezo buzzer, and can be configured using the web app to sound when any measured quantity either exceeds or decreases below a set threshold.

## Powering the device

The device can be powered either with a 5V power supply plugged into the 2.1/5mm jack, or with a micro USB cable connected to a computer or other power source. If both are connected, only the jack will be used.
