# R.O.A.D.S — Real-Time Onboard Anomaly Detection System

An IoT-based road anomaly detection system that transforms vehicles into 
intelligent mobile road condition monitoring nodes.

## Overview

R.O.A.D.S. captures real-time vehicle vibration data using an MPU6050 IMU 
sensor, classifies road conditions via Edge AI on an ESP32-S3 microcontroller, 
and transmits results via Bluetooth Low Energy (BLE) to an Android 
application for visualization and cloud logging.

## System Architecture

[Vehicle] → [MPU6050 Sensor] → [ESP32-S3 + Edge AI] → [BLE] → 
[Android App] → [Firebase Realtime Database]

## Key Results

- **Classification Accuracy:** 100% (F1 Score: 1.00)
- **Model:** Quantized int8 neural network (39 features → 2 dense layers → 3 classes)
- **Sampling Rate:** 77Hz
- **Classes:** Bumpy, Potholes, Smooth Road

## Technologies Used

| Component | Technology |
|-----------|-----------|
| Hardware | Cytron Maker Feather AIoT S3 (ESP32-S3), MPU6050 |
| Edge AI | Edge Impulse Studio |
| Mobile App | Android (Kotlin), custom Canvas rendering |
| Cloud | Firebase Realtime Database |
| Communication | Bluetooth Low Energy (BLE) |

## Project Report

Full technical documentation available in the repository.

## Acknowledgements

Final Year Project — Diploma in Computer Science  
Kolej Poly-Tech MARA (KPTM) Alor Setar, 2026


