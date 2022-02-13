---
layout: post
title: IoT - Room Tempearture
date: 2022-02-12
categories: jekyll update
excerpt_separator: <!--more-->
---

The goal of this project is to find the difference of the room's temperature and humidity in different areas of the apartment. Temperature and humidity are collected by sensors which are located in different areas of the apartment. A server is needed to collect the data and store in a local database. The data will then be analysed.

Project can be split into 3 parts

Part 1 - Sensors

Breadboard Schematic Diagram shown below are set up to flash the ESP-01S module. Arduino IDE is used to upload the sketch and flash the ESP-01S module.

![Breadboard](/assets/IoTRoomTemperature/flashing-esp01s_bb.png)
![Schematic](/assets/IoTRoomTemperature/flashing-esp01s_schem.PNG)

Technologies and Tools Used
- Arduino IDE
- ESP-01S
- ESP8266(ESPF-DEVKIT V4)
- DHT 11

Part 2 - Django Server and Database
<!-- - [C++ implementation for inverse and division](https://github.com/kinming92/divvy_assembler) -->
<!-- - [Final Code](https://github.com/kinming92/Divvy_FinalProject) -->

Part 3 - Analytic Report