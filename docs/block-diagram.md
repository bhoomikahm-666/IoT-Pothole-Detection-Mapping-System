# System Block Diagram

## IoT-Based Real-Time Pothole Detection and Mapping System

The system integrates vibration sensing, GPS-based location tracking, embedded processing and cloud-based visualization.

          Road Vibration
                |
                v
        +----------------+
        |    MPU6050     |
        | Accelerometer |
        +----------------+
                |
               I2C
                |
                v
        +----------------+
        |      ESP32     |
        | Data Processing|
        +----------------+
                ^
                |
             UART
                |
        +----------------+
        |   GPS Neo-6M   |
        +----------------+

                |
                v
          Wi-Fi Network
                |
                v
        +----------------+
        | ThingSpeak /   |
        | Data Services  |
        +----------------+
                |
                v
        +----------------+
        | Django Backend |
        | Data Processing|
        +----------------+
                |
                v
        +----------------+
        | Web Map and    |
        | Email Alerts   |
        +----------------+
```

## Data Flow

1. The MPU6050 measures acceleration and vibration.
2. The ESP32 processes sensor readings and evaluates the configured detection threshold.
3. GPS coordinates are obtained from the Neo-6M module.
4. The ESP32 transmits event data through Wi-Fi.
5. Cloud services and backend processing support data organization.
6. The web interface displays recorded locations and the system generates email notifications.

