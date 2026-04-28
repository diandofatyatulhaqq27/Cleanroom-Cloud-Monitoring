# Cleanroom-Cloud-Monitoring

#Cleanroom Prototype Cloud Monitoring System
An advanced industrial IoT prototype designed for real-time monitoring and automated environmental control in cleanroom facilities. This project bridges the gap between traditional industrial automation (PLC/SCADA) and modern cloud-based data visualization.

#📌 Overview
Cleanrooms require stringent environmental control to prevent contamination. This system monitors air quality, gas levels, and pressure while automating Honeywell Damper Actuators to maintain safety and ISO standards. Data is pushed to the cloud via MQTT for remote monitoring and historical audit trails.

#🚀 Key Features
*Real-time Environmental Monitoring: Tracks gas concentrations (%LEL) and ventilation status.
*Intelligent Damper Control: Implements Off-Delay Timers and Hysteresis logic to prevent motor "hunting" and extend hardware lifespan.
*Cloud Integration: Integrated with Haiwell Cloud SCADA for remote access via mobile or web.
*Fail-Safe Design: Support for Spring Return actuators to ensure immediate sealing during power or system failures.
*Historical Data Logging: Automated record-keeping for environmental compliance and trend analysis.

#🛠️ Technical Stack
*Controller: Haiwell PLC AT16S0R, Haiwell PLC Expand A04AI, Haiwell HMI B7H-W.
*Actuators: Pilot Lamp Buzzer, PC Fan 8x8.
*Sensors: Signal Generator x2
*Protocols: MQTT, Modbus TCP/IP
*Monitoring: Haiwell Cloud SCADA, Grafana (via Telegraf & InfluxDB)

#📐 System Architecture
*Field Layer: Sensors and Actuators connected to PLC Digital/Analog I/O.
*Control Layer: PLC processes logic (Timer Off-Delay, Interlocking).
*Transport Layer: Data transmission via MQTT Broker.
*Application Layer: Cloud Dashboard for visualization and History Record management.
