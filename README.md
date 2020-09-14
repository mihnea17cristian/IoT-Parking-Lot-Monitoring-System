# IoT-Parking-Lot-Monitoring-System
IoT monitoring system that uses multiple sensors and technologies 

This IoT monitoring system uses ESP8266 and ESP32 microcontrollers to monitor parking spots availability. The MCUs act as data acquisition nodes for the spot's state (free/reserved/occupied). Using MQTT messages, the nodes send updates to the central server, which consists of a RaspberryPi. This server stores the information in an InfluxDB database and uses Grafana to plot data to users. The MQTT messages are received by the RaspberryPi using Mosquitto broker and Telegraf.
