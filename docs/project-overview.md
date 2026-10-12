# IoT-Based Real-Time Pothole Detection and Mapping System

## 1. Project Overview

This project uses an ESP32-based embedded IoT system to detect potential pothole events using road vibration data, capture GPS coordinates and visualize recorded locations through a web-based map.

## 2. Objectives

- Detect abnormal road vibrations using an MPU6050 sensor.
- Capture location coordinates using a GPS Neo-6M module.
- Process sensor readings using the ESP32.
- Transmit event data over Wi-Fi.
- Store and process data using the configured cloud and backend services.
- Display recorded locations on a map.
- Generate email alerts containing location information.

## 3. Hardware Components

- ESP32 microcontroller
- MPU6050 accelerometer and gyroscope
- GPS Neo-6M module
- TP4056 charging module
- MT3608 boost converter
- Lithium-ion battery

## 4. Software and Technologies

- Arduino IDE and embedded C/C++
- I2C and UART communication
- ESP32 Wi-Fi
- ThingSpeak
- Django and Python
- Google Sheets
- Web-based map visualization

## 5. Working Methodology

1. The MPU6050 measures road vibration and acceleration.
2. The ESP32 evaluates sensor readings against a configured threshold.
3. The GPS module supplies coordinates when a valid GPS fix is available.
4. The ESP32 transmits event information through Wi-Fi.
5. The cloud and backend components support data storage and processing.
6. The web interface visualizes recorded locations.
7. The system generates email notifications containing location information.

## 6. Results

The project demonstration includes a live pothole data table, geographical coordinates, a map visualization, and automated email notifications. The hardware prototype was also documented during a road-testing setup.

Refer to the `../results/` folder for screenshots and hardware evidence.

## 7. Limitations

Speed breakers and uneven road surfaces may produce false detections. Threshold-based filtering was used to reduce unnecessary detections.

## 8. Future Enhancements

- Improve vibration filtering and event classification.
- Evaluate the system across additional road conditions.
- Improve duplicate-event handling.
- Enhance map visualization and reporting.

## 9. Project Evidence

- Hardware photographs and circuit diagram: `../hardware/`
- Test results and screenshots: `../results/`
- System block diagram: `block-diagram.md`
- Detection workflow: `flowchart.png`

## 10. Author

Bhoomika H M  
Electronics and Communication Engineering  
Sir M. Visvesvaraya Institute of Technology

*This document summarizes the project. Refer to the actual source code and circuit schematic for implementation-specific details.*
