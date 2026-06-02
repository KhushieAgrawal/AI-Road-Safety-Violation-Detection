
# AI-Powered Road Safety Violation Detection System

## Overview

An AI-powered surveillance system designed to automatically detect road safety violations in campus environments. The system combines Computer Vision, Deep Learning, OCR, IoT, and Cloud Computing to identify helmet and seatbelt violations, extract vehicle license plate information, and maintain automated violation records.

The solution aims to reduce manual monitoring efforts while promoting safer road practices through intelligent and scalable traffic surveillance.

---

## Problem Statement

Monitoring road safety violations manually is time-consuming, resource-intensive, and prone to human error. Educational campuses and private premises often lack automated systems to detect violations such as riding without helmets or driving without seatbelts.

This project aims to provide an AI-driven solution that automates violation detection, license plate recognition, and record maintenance in real time.

---

## Features

* Vehicle detection and classification
* Helmet violation detection for two-wheelers
* Seatbelt violation detection for four-wheelers
* Automatic license plate detection
* OCR-based license plate reading
* Google Sheets-based violation logging
* Raspberry Pi and camera integration
* Cloud deployment using Hugging Face Spaces
* Real-time monitoring dashboard

---

## Tech Stack

### Programming Language

* Python

### Computer Vision & Deep Learning

* YOLOv8 (Ultralytics)
* OpenCV

### OCR

* EasyOCR

### Cloud & Deployment

* Hugging Face Spaces
* FastAPI
* Gradio

### IoT & Hardware

* Raspberry Pi 4
* PIR Motion Sensor
* Pi Camera Module

### Database & Logging

* Google Sheets API
* Google Drive

---

## Methodology

### 1. Vehicle Detection

* Images are captured using a Raspberry Pi camera.
* A pre-trained YOLOv8 COCO model detects vehicles.

### 2. Violation Detection

* Helmet detection model checks compliance for two-wheelers.
* Seatbelt detection model checks compliance for four-wheelers.

### 3. License Plate Recognition

* License plate detection model localizes the number plate.
* EasyOCR extracts the plate text.

### 4. Violation Logging

* Detected violations are automatically logged to Google Sheets with timestamp, vehicle type, violation type, and plate number.

---

## System Workflow

```text
Vehicle Detection
        ↓
Vehicle Classification
        ↓
 ┌──────────────┬
 ↓              ↓
Two-Wheeler   Four-Wheeler
 ↓              ↓
Helmet Check  Seatbelt Check
        ↓
Violation Detected
        ↓
License Plate Detection
        ↓
Google Sheets Logging
```

---

## Models Used

| Model          | Purpose                 |
| -------------- | ----------------------- |
| YOLOv8n (COCO) | Vehicle Detection       |
| YOLOv8s        | Helmet Detection        |
| YOLOv8s        | Seatbelt Detection      |
| YOLOv8s        | License Plate Detection |
| EasyOCR        | License Plate Reading   |

---

## Results

* Automated detection of helmet and seatbelt violations.
* Accurate vehicle classification using a COCO pre-trained model.
* Automated license plate extraction and OCR processing.
* Cloud-based violation logging and monitoring.
* Scalable architecture suitable for smart campus deployment.

---

## Project Structure

```text
AI-Road-Safety-System/
│
├── datasets/
├── models/
├── scripts/
│   ├── download_datasets.py
│   ├── merge_datasets.py
│   ├── fix_labels.py
│   └── train_all_models.py
│
├── yaml/
├── app.py
├── requirements.txt
├── Dockerfile
└── README.md
```

---

## Future Improvements

* Night-time violation detection
* Multi-camera support
* Mobile application for administrators
* Speed violation monitoring
* Offline edge deployment on Raspberry Pi
* Real-time analytics dashboard

---

## Intellectual Property

An **Annexure II – Invention Disclosure Form (IDF)** has been submitted for this project under the Intellectual Property and Innovation initiative of Symbiosis Institute of Technology, Pune.

---

## Contributors

* Khushie Agrawal
* Shriya Kurup
* Akarsh Sunil


---

## Impact

The project demonstrates the practical application of Artificial Intelligence, Computer Vision, and IoT in enhancing road safety. By automating violation detection and record management, it contributes toward smarter, safer, and more efficient campus traffic monitoring systems. 

