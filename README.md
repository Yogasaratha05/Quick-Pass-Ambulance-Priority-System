# Quick Pass – Ambulance Priority Traffic Control System

## Project Description

Quick Pass is an IoT-based ambulance traffic priority prototype designed to help identify ambulances using RFID technology and provide zone-based traffic alerts.

The system uses an ESP8266 NodeMCU to communicate with an RFID reader, LCD display, buzzer, and a web dashboard. Users can select traffic zones through the dashboard and view the current system status.

## Objectives

* Identify ambulance RFID tags.
* Display ambulance identification and zone messages on an LCD.
* Generate buzzer alerts for selected traffic zones.
* Provide a web-based interface to monitor system status.
* Demonstrate an IoT-based approach to ambulance traffic priority management.

## Hardware Components

* ESP8266 NodeMCU
* MFRC522 RFID reader
* RFID tag or card
* 16x2 I2C LCD display
* Buzzer
* Connecting wires
* USB power supply

## Software Requirements

* Arduino IDE
* ESP8266 board package
* MFRC522 library
* LiquidCrystal_I2C library
* ESP8266WiFi library
* ESP8266WebServer library

## Features

* RFID tag scanning
* Ambulance ID display
* Wi-Fi connectivity
* Web dashboard for system monitoring
* Manual traffic-zone selection
* Zone-based buzzer alerts

## Traffic Zones

1. NORMAL – Clear Route
2. SCHOOL_ZONE – School zone alert
3. ACCIDENT_ZONE – Accident caution
4. TRAFFIC_HEAVY – Heavy traffic alert

## Working Principle

1. The MFRC522 reader scans an RFID tag.
2. The ESP8266 reads and stores the tag ID.
3. The LCD displays the ambulance ID and selected zone message.
4. The web dashboard displays the system status.
5. The buzzer provides alerts when an alert zone is selected and an RFID tag has been detected.

## Limitations

* The current prototype uses manual zone selection.
* RFID scanning identifies a tag but does not independently verify that the vehicle is an authorized ambulance.
* The system does not directly control real traffic signals.
* Wi-Fi credentials must be configured before operation.
* The buzzer and zone logic require hardware testing.

## Future Enhancements

* GPS-based ambulance location tracking
* Automatic traffic-zone detection
* Integration with traffic signal controllers
* Authorized RFID tag verification
* Mobile-friendly monitoring dashboard

## Project Status

Prototype implementation — hardware testing and further validation required.

## Disclaimer

This project is intended for educational and demonstration purposes. It is not a deployed emergency traffic management system.
