# Power IoT Resources

Microsoft Power Apps samples using the [Pilot Things](https://www.pilot-things.com) Power IoT connector to integrate IoT sensor data into business applications.

## Overview

This repository contains Power Apps samples that demonstrate how to build IoT-enabled applications using the Pilot Things connector and Device Explorer cloud service. The samples show how to visualize and manage IoT sensor data without writing code, leveraging the power of Microsoft Power Platform.

## What's Included

### 📱 Sample Applications

- **AdeunisFTD**: Display Adeunis Field Test Device (FTD) GPS trackers on an interactive map with real-time location data

### 📦 Component Libraries

- **Sensor Twins**: Reusable component library with pre-built sensor controls that you can integrate into your own Power Apps

### 🔌 Pilot Things Connector

The Pilot Things connector enables you to:
- View and manage your IoT devices (things)
- Access real-time sensor measurements
- Monitor device statistics and alerts
- Perform device operations
- Integrate sensor data models with business applications

## Prerequisites

Before using these samples, you'll need:

### 1. Device Explorer Account

You must have an active [Device Explorer](https://www.pilot-things.com/iot-sensor-apps/device-explorer) account from Pilot Things. Device Explorer is a cloud service that:
- Manages your IoT sensor fleet
- Associates data models with sensors
- Provides real-time data access
- Enables integration with business applications and AI/LLM services

[Sign up for Device Explorer](https://www.pilot-things.com/iot-sensor-apps/device-explorer)

### 2. Microsoft Power Apps License

- Power Apps license (Premium connectors require appropriate licensing)
- Access to your organization's Power Apps environment

### 3. Pilot Things Connector Setup

The Pilot Things connector must be configured in your Power Apps environment. The connector is available in the Microsoft Power Platform connector catalog.

## Getting Started

### Step 1: Import the Sample App

1. Download the sample you want to use from the `samples/` folder
2. Open [Power Apps Studio](https://make.powerapps.com)
3. Click **Apps** > **Import canvas app**
4. Upload the sample package
5. Follow the import wizard

### Step 2: Configure Connections

After importing, you'll need to configure the following connections:

1. **Pilot Things Connection**
   - Add your Device Explorer credentials
   - Configure the connection to point to your Pilot Things instance

2. **Additional Connections** (for AdeunisFTD sample)
   - Microsoft Spatial Services (for map functionality)
   - Power Apps for Makers (optional, for app management)

### Step 3: Customize and Run

1. Update data sources to point to your devices
2. Customize the UI to match your branding
3. Add additional functionality as needed
4. Save and publish your app

## Sample Details

### AdeunisFTD Sample

This sample demonstrates GPS tracking visualization for Adeunis Field Test Device (FTD) sensors.

- **Features**:
  - Device list view with status indicators
  - Interactive map with device locations
  - Real-time temperature and GPS measurements
  - Device details screen

- **Implementation**:
  - Built with standard Power Apps controls (no component library dependencies)
  - Direct integration with Pilot Things connector APIs
  - Uses Microsoft Spatial Services for map visualization

- **Data Sources**:
  - Pilot Things connector for device data
  - Microsoft Spatial Services for mapping

- **Use Cases**:
  - Fleet tracking
  - Asset location monitoring
  - Field service management

**Note**: This sample does not use the SensorTwins component library. It's a standalone app built with native Power Apps controls.

### Sensor Twins Component Library

A reusable Power Apps component library designed to accelerate IoT app development.

- **What it includes**:
  - Pre-built sensor visualizations
  - Standardized data binding for Device Explorer
  - Customizable styling and themes
  - Ready-to-use sensor controls

- **How to use**:
  - Import the component library into your Power Apps environment
  - Add components to your canvas apps
  - Connect to your Device Explorer data sources
  - Customize appearance to match your branding

- **Benefits**:
  - Faster development time
  - Consistent UI across apps
  - Best practices built-in
  - Easy integration with Pilot Things connector

## Architecture

```
Power Apps ←→ Pilot Things Connector ←→ Device Explorer ←→ IoT Sensors
```

The Pilot Things connector bridges IoT devices with the no-code Power Platform, enabling you to build sensor-enabled applications without custom development.

## Resources

- [Pilot Things Website](https://www.pilot-things.com)
- [Device Explorer Documentation](https://www.pilot-things.com/iot-sensor-apps/device-explorer)
- [Power IoT Overview](https://www.pilot-things.com/en/iot-sensor-apps/power-iot)
- [Microsoft Power Apps Documentation](https://docs.microsoft.com/powerapps/)
- [Pilot Things Connector - Official Microsoft Documentation](https://docs.microsoft.com/en-us/connectors/pilotthings/)

## Support

For issues related to:
- **Device Explorer or Pilot Things connector**: Contact [Pilot Things Support](https://www.pilot-things.com)
- **Power Apps platform**: Refer to [Microsoft Power Apps Support](https://powerapps.microsoft.com/support/)
- **Sample apps in this repository**: Open an issue on GitHub

## Contributing

Contributions are welcome! If you've built interesting IoT applications using Pilot Things and Power Apps, feel free to submit a pull request with your samples.

## License

See [LICENSE](LICENSE) file for details.

---

Built with ❤️ using Microsoft Power Platform and Pilot Things Power IoT
