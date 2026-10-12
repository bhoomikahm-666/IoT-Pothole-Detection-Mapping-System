# Hardware Components

## 1. ESP32 Microcontroller
The ESP32 acts as the main controller. It reads sensor data, processes detection events and transmits information through Wi-Fi.

## 2. MPU6050 Accelerometer and Gyroscope
The MPU6050 measures acceleration and vibration along three axes. The ESP32 uses these readings to identify abnormal vibration events based on a predefined threshold.

## 3. GPS Neo-6M Module
The GPS module provides latitude and longitude coordinates to associate detected events with geographical locations.

## 4. TP4056 Charging Module
Used in the project's documented battery charging arrangement.

## 5. MT3608 Boost Converter
Used for DC-DC voltage conversion in the power supply circuit.

## 6. Lithium-Ion Battery
Provides portable power to the hardware system.

## 7. Hardware Communication

- **I2C:** Communication between the ESP32 and MPU6050.
- **Serial/UART:** Communication between the ESP32 and GPS Neo-6M.
- **Wi-Fi:** Transmission of event data to the cloud.

## System Overview

The ESP32 collects vibration data from the MPU6050, evaluates the readings against a configured threshold, obtains GPS coordinates for detected events and sends event information to the cloud using Wi-Fi.

Refer to `circuit-diagram.png` for the actual hardware connections.
