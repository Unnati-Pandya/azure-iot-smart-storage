# Azure IoT Smart Storage System

A hybrid smart storage solution built using azure IoT Hub, Blob Storage and Time Series Insights.
The system ingests real-time device telemetry, enforces secure access, and automates on business logic.


## Key Features
## 1. Secure Device Communication
- Azure IoT Hub for bidirectional messaging
- Microsoft Entra ID (Azure AD) for role-based access
- Device identity provisioning and authentication
- Scalable IoT architecture
- Time series diagnostics

## 2. Real-Time data processing
- Azure Functions to automate threshold alerts
- Event Grid for event-driven workflows and device lifecycle management
- Time Series Insights to visualize historical and real-time metrics

## 3. Storage & Cost Optimization
- Azure Blob storage to store device data
- Policies to reduce unnecessary data flow and storage usage

## Architecture Flow
* Devices -> IoT Hub -> Event Grid -> Azure Functions -> Storage / Insights *
- Device telemetry flows to IoT Hub
- Events (tempreture, capacity, errors) triggers Azure Functions
- Alerts or commands are then sent back to devices
- Data archived and visualized in Time Series Insights

  ## Outcomes
- Reduced unnecessary device communication
- Automated alerts for abnormal conditions
- Improved visibility into IoT system health
- Modular design for scaling more devices or sensors
