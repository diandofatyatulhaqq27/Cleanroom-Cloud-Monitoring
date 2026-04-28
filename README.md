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

# HaiwellHappy
*Notes: This is only some screenshot of the full ladder diagram
<img width="1171" height="475" alt="Visual" src="https://github.com/user-attachments/assets/44576593-ab35-4699-a92b-782e2db55dda" />
<img width="1138" height="572" alt="Control" src="https://github.com/user-attachments/assets/8444bf07-e8a6-427d-bc13-edd73b8dc704" />
<img width="1183" height="666" alt="Register" src="https://github.com/user-attachments/assets/12847339-3bd2-4e25-8ee3-da5b1bfddbb6" />

# HaiwellSCADA
<img width="1282" height="749" alt="image" src="https://github.com/user-attachments/assets/465e67a5-f73f-4f0a-934b-3767879a3047" />
<img width="1279" height="754" alt="image" src="https://github.com/user-attachments/assets/d95909ba-7807-4657-9edf-a56373f10006" />






