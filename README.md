# IoT-Parking-Lot-Monitoring-System
IoT monitoring system that uses multiple sensors and technologies 

This IoT monitoring system uses ESP8266 and ESP32 microcontrollers to monitor parking spots availability. The MCUs act as data acquisition nodes for the spot's state (free/reserved/occupied). Using MQTT messages, the nodes send updates to the central server, which consists of a RaspberryPi. This server stores the information in an InfluxDB database and uses Grafana to plot data to users. The MQTT messages are received by the RaspberryPi using Mosquitto broker and Telegraf.

Lucrarea completă necesită dezvoltarea următoarelor componente:
• Serverul local de monitorizare, găzduit de placa RaspberryPi;
• Baza de date, aferentă sistemului;
• Sistemul de comunicație între senzori, microcontrolere și placa RaspberryPi;
• Sistemul de transmitere a datelor către un server central extern, pe bază de apeluri REST.


