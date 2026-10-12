# IoT-Pothole-Detection-Mapping-System

PROJECT OVERVIEW

An ESP32-based embedded and IoT system designed to detect potholes using road vibration data, capture their geographical coordinates and visualize detected locations on a web-based map.
The system integrates motion sensing, GPS tracking, Wi-Fi communication, cloud data storage and backend processing to support real-time road-condition monitoring.

PROBLEM STATEMENT

Manual road inspection is time-consuming and makes it difficult to continuously identify and record pothole locations. This project explores an embedded IoT solution to automate pothole detection and location mapping.

OBJECTIVES

Detect abnormal road vibrations using an MPU6050 accelerometer.
Capture geographical coordinates using a GPS Neo-6M module.
Process sensor data using the ESP32 microcontroller.
Transmit detected events over Wi-Fi.
Store and monitor data using ThingSpeak and Google Sheets.
Use Django backend processing to filter duplicate records.
Visualize detected pothole locations on a custom web map.
Generate email notifications for detected pothole events.

HARDWARE COMPONENTS

ESP32 microcontroller
MPU6050 accelerometer and gyroscope
GPS Neo-6M module
TP4056 battery charging module
MT3608 boost converter
Lithium-ion battery
Connecting wires and associated hardware

SOFTWARE AND TECHNOLOGIES

Arduino IDE and embedded C/C++ for ESP32 firmware
I2C communication for the MPU6050
Serial communication for GPS data
Wi-Fi connectivity
ThingSpeak and Google Sheets for data storage and monitoring
Django for backend processing
Web-based map visualization

SYSTEM ARCHITECTURE

The MPU6050 continuously measures acceleration and vibration.
The ESP32 evaluates sensor readings against predefined threshold conditions.
When an abnormal vibration is detected, the GPS module provides the current coordinates.
The ESP32 transmits the event data through Wi-Fi.
Cloud storage and backend processing organize the collected records and filter duplicates.
The processed location data is displayed on a web-based map.
Email notifications provide additional awareness of detected events.

RESULTS AND TESTING

The project report documents testing under different road conditions. The system detected many pothole events, captured corresponding GPS coordinates and transmitted the data for visualization.
False detections could occur on speed breakers and uneven road surfaces. Threshold-based filtering was used to reduce unnecessary detections.

APPLICATIONS

Road-condition monitoring
Smart-city infrastructure projects
Pothole location mapping
IoT-based transportation monitoring
Embedded systems and sensor-integration demonstrations

FUTURE ENCHANCEMENTS

Improve detection using calibrated thresholds and sensor-data filtering.
Evaluate detection accuracy across more road conditions.
Introduce improved event validation and duplicate detection.
Extend the mapping interface and reporting capabilities.

PROJECT EVIDENCE

Hardware prototype: hardware/prototype.jpg
Circuit diagram: hardware/circuit-diagram.png
Cloud dashboard: results/cloud-dashboard.png
Map output: results/map-output.png
Project overview: docs/project-overview.pdf

Author

Bhoomika H M
Electronics and Communication Engineering
Sir M. Visvesvaraya Institute of Technology
