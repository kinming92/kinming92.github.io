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
![Schematic](/assets/IoTRoomTemperature/flashing-esp01s_schem.png)

Technologies and Tools Used
- Arduino IDE
- ESP-01S
- ESP8266(ESPF-DEVKIT V4)
- DHT 11

Part 2 - Django REST API and Database

The REST API is designed for the ESP-01S module clients to send request to the server. The hosted server will be responsible to take the data from http request and store the data into the database.

Database Design from Draw.io
![database-design](/assets/IoTRoomTemperature/web-sensor-api-database-design.drawio.png)


Technologies and Tools Used
- Django Rest Framework
- SQLite3

Part 3 - Guide to Deloy the Django + Gunicorn + Nginx in Ubuntu Server

[Install Ubuntu Server and Enable SSH ](https://ubuntu.com/tutorials/how-to-install-ubuntu-on-your-raspberry-pi#4-boot-ubuntu-server)
[Setup Django + Gunicorn + Nginx in Ubuntu Server](https://www.digitalocean.com/community/tutorials/how-to-set-up-django-with-postgres-nginx-and-gunicorn-on-ubuntu-22-04)

Part 4 - Analytic Report