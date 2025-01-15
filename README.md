# 🚗 Vehicle Tracking and Speed Estimation Using OpenCV

This repository contains the implementation of a Vehicle Tracking and Speed Estimation system using OpenCV and Python. The project leverages Computer Vision techniques to detect, track, and estimate the speed of vehicles in video feeds, with potential applications in traffic law enforcement and congestion management.

## 📖 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Workflow](#workflow)
- [Usage](#usage)
- [Results](#results)
- [Future Enhancements](#future-enhancements)
- [Contact](#contact)

## 📋 Overview
Traffic monitoring is a critical aspect of urban management, but manual methods are prone to errors and inefficiencies. This project automates the process using Computer Vision to deliver:
- Accurate vehicle detection.
- Real-time speed estimation.
- Insights for smarter traffic management.

## 🌟 Features
- **Vehicle Detection**: Uses background subtraction and contour detection to identify vehicles.
- **Real-Time Tracking**: Assigns unique IDs to track vehicles across frames.
- **Speed Estimation**: Calculates speed in km/h using pixel-to-meter conversion.
- **Preprocessing Pipeline**: Implements grayscale conversion, Gaussian blur, and morphological transformations for noise reduction.

## 🛠️ Workflow
1. **Video Input**: Load a video feed or camera input.
2. **Preprocessing**: Grayscale conversion, Gaussian blur, and background subtraction.
3. **Morphological Transformations**: Dilate and close regions to refine detected objects.
4. **Contour Detection**: Identify vehicle boundaries.
5. **Tracking**: Assign unique IDs to vehicles and update positions.
6. **Speed Estimation**: Calculate speed using distance traveled over time.
7. **Output**: Display results with bounding boxes and speed annotations.

## 🚀 Usage
Replace the video file in the code with your desired input:
```python
cap = cv2.VideoCapture('input_video.mp4')  
