# Automatic Number Plate Recognition (ANPR) System

## Introduction
This project focuses on the development and implementation of an Automatic Number Plate Recognition (ANPR) system. ANPR systems have become widely used for safety, security, and commercial purposes. The core of this project is based on the SSD Mobnet, with a pre-trained model customized to undergo 10,000 training steps. This technology aims to automate the manual process of checking and registering vehicle number plates, which can enhance security and reduce manual labor.

## Features
- **Image Capture**: Captures images using a 5MP camera.
- **Image Processing**: Converts captured images into binary format to increase processing speed.
- **Model Training**: Uses the SSD Mobnet model for detecting vehicle number plates.
- **Text Extraction**: Utilizes EasyOCR for extracting text from the trained image.

## Problem Definition
The manual checking and registering of vehicle number plates in environments such as universities can lead to security issues and increased labor. By introducing an ANPR system, safety can be assured, and manual work can be significantly reduced.

## Project Components

### SSD Mobnet
The SSD (Single Shot MultiBox Detector) model has two main components:
1. **Backbone Model**: Typically a pre-trained image classification network like ResNet trained on ImageNet, used as a feature extractor. It extracts semantic meaning from the input image while preserving its spatial structure.
2. **SSD Head**: Responsible for detecting objects and their locations by matching anchor boxes with ground truth bounding boxes.

### Recognition Process
The recognition process consists of three main steps:
1. **Region of Interest Extraction**: Identifying the area of the image that contains the license plate.
2. **Plate Number Extraction**: Isolating the license plate from the image.
3. **Character Recognition**: Reading and identifying the characters on the license plate using EasyOCR.

## Technologies Used
- **Platform**: Visual Studio Code (VSCode)
- **Programming Language**: Python
- **Libraries and Tools**:
  - OpenCV
  - TensorFlow
  - Object Detection API
  - EasyOCR

## Setup Instructions
1. **Clone the Repository**:
    ```sh
    git clone [repository URL]
 
