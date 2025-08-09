# Home Automation using IoT

*Author:* Juthuka Naina  
*Year:* 2025

## Overview
A simple and reliable home automation system that allows remote monitoring and control of household appliances. The system uses microcontroller-based nodes and a Wi‑Fi/MQTT link to a lightweight dashboard, enabling automation for lighting, fan control, and basic security sensing.

## Key Features
- Remote ON/OFF control of appliances (lights, fans)  
- Sensor-based automation (motion / light / temperature triggers)  
- Basic scheduling and manual control via a web/mobile dashboard  
- Data logging for device status and sensor readings

## Technologies & Tools
- *Hardware:* Arduino Uno / ESP8266 (NodeMCU) / Relay module / DHT11 / PIR sensor / LDR  
- *Software:* Arduino IDE, MQTT broker (Mosquitto), simple web dashboard (Flask / Node.js / plain HTML+JS)  
- *Communication:* MQTT over Wi‑Fi

## Hardware List (example)
- Arduino Uno or NodeMCU (ESP8266) — 1  
- 5V Relay Module — 1 (or more for multiple appliances)  
- DHT11 Temperature & Humidity Sensor — 1  
- PIR Motion Sensor — 1  
- LDR (light sensor) — 1  
- Jumper wires, breadboard, power supply

## My Role
I designed and implemented the hardware integration and core firmware, connected sensors and relays, and implemented the MQTT communication. I also helped build a simple web interface for manual control and status monitoring.

## How it works (summary)
1. Sensors read environment data (temperature, motion, light).  
2. Microcontroller publishes sensor data to an MQTT broker.  
3. Dashboard subscribes to topics and shows real-time status.  
4. User commands from the dashboard are published to control topics; microcontroller receives these and switches relays accordingly.  
5. Optional automation rules run on the microcontroller or the dashboard (e.g., turn ON light if PIR triggered after sunset).

## Setup (quick)
1. Configure and run an MQTT broker (e.g., Mosquitto) on local PC or cloud.  
2. Open firmware/ in Arduino IDE,
# HOME_AUTOMATION_IOT
Iot_based home automation system to control and monitor appliances remotely using sensors and microcontrollers.
