# Cleanroom-Cloud-Monitoring

# Cleanroom Prototype Cloud Monitoring System
An advanced industrial IoT prototype designed for real-time monitoring and automated environmental control in cleanroom facilities. This project bridges the gap between traditional industrial automation (PLC/SCADA) and modern cloud-based data visualization.

# 📌 Overview
Cleanrooms require stringent environmental control to prevent contamination. This system monitors air quality, gas levels, and pressure while automating Honeywell Damper Actuators to maintain safety and ISO standards. Data is pushed to the cloud via MQTT for remote monitoring and historical audit trails.

# 🚀 Key Features
* Real-Time Environmental Monitoring: Precise tracking of critical cleanroom parameters, including temperature, humidity, and the operational status of fans and heaters to maintain strict environmental standards.
* Intelligent Fan & Heater Control: Automated HVAC management using PLC logic to ensure a stable, controlled environment based on user-defined setpoints.
* Advanced Stability Logic: Implementation of Hysteresis and Off-Delay Timers to prevent "hunting" (rapid on/off cycling). This logic ensures thermal stability and significantly extends the operational lifespan of the hardware.
* Global Cloud Integration (GCP Powered): Infrastructure hosted on Google Cloud Platform (GCP), enabling worldwide monitoring capabilities. The system operates independently of local network (LAN) restrictions, allowing secure access from any location via a public internet connection.
* End-to-End Industrial IoT Pipeline: A robust data architecture that pushes JSON-formatted industrial data via MQTT to a cloud-based stack consisting of Telegraf, InfluxDB, and Grafana.
* Dynamic Data Visualization: High-performance Grafana Dashboards that provide real-time visual analytics, historical trend mapping, and automated alerting systems for 24/7 surveillance.

Historical Compliance Logging: Automated data archiving within InfluxDB to facilitate audit trails, environmental compliance reporting, and long-term system performance analysis.

# 🛠️ Technical Stack
* Controller: Haiwell PLC AT16S0R, Haiwell PLC Expand A04AI, Haiwell HMI B7H-W.
* Actuators: Pilot Lamp Buzzer, PC Fan 8x8.
* Sensors: Signal Generator x2
* Protocols: MQTT, Modbus TCP/IP
* Monitoring: Haiwell Cloud SCADA, Grafana (via Telegraf & InfluxDB)

# 📐 System Architecture
* Field Layer: Sensors and Actuators connected to PLC Digital/Analog I/O.
* Control Layer: PLC processes logic (Timer Off-Delay, Interlocking).
* Transport Layer: Data transmission via MQTT Broker.
* Application Layer: Cloud Dashboard for visualization and History Record management.

# Demo Video


https://github.com/user-attachments/assets/829cdfd1-ad28-4b8c-a8ee-0c5dcade0b37





