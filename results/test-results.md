# Test Results and Validation

## 1. Sensor Data Acquisition

The MPU6050 accelerometer provides acceleration and vibration readings to the ESP32. These readings are used to identify abnormal vibration events.

## 2. Pothole Event Detection

The ESP32 compares sensor readings against a configured threshold to identify potential pothole events.

## 3. GPS Location Tracking

The GPS Neo-6M module provides latitude and longitude coordinates associated with detected events, when a valid GPS fix is available.

## 4. Cloud Data Transmission

The ESP32 uses Wi-Fi to transmit event information to the configured cloud platform for storage and monitoring.

## 5. Map Visualization

The processed location records are displayed on a web-based map to help visualize detected pothole locations.

## Limitations

Speed breakers and uneven road surfaces may cause false detections. Threshold-based filtering was used to reduce unnecessary detections.

