https://github.com/user-attachments/assets/9cd01544-281f-4dc6-92ce-8ced66a305c8

# Smart Waste Segregation

## Overview
The **Smart Waste Segregation** project leverages machine learning and object detection to automate the process of waste segregation and classification. This project utilizes the Ultralytics YOLOv8 model for object detection, AutoDistill for image segmentation, and GroundedSAM for annotation. The entire workflow, including model training and data preprocessing, is executed using Python scripts and CLI commands in Google Colab, leveraging the power of a T4 GPU.

## Introduction
The project aims to develop an efficient waste segregation system using advanced machine learning techniques. By employing object detection and image segmentation, the system can accurately classify and segregate different types of waste.

## Features
- **Object Detection**: Utilizes YOLOv8 for detecting various waste items.
- **Image Segmentation**: Uses AutoDistill and GroundedSAM for precise segmentation and annotation.
- **Real-time Testing**: Implements OpenCV2 for real-time webcam testing.
- **GPU Acceleration**: Leverages T4 GPU in Google Colab for faster processing.

## Installation
To set up the project, follow these steps:
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/smart-waste-segregation.git
    cd Smart-Waste-Segregation-Project-main
    ```
2. Install dependencies using commmands mentioned in `Annotator.ipynb` and `trainingModel.ipynb` (for training).

## Usage
1. To directly see how this model works, you can run `best_overall.pt`.
2. To train the model on custom dataset (already annotated), feed them directly into the model using `trainingModel.ipynb`.
3. Incase dataset is not annotated already, use `Annotator.ipynb` for annotating the dataset and then train the model using `trainingModel.ipynb`.
4. After all this training, validation and testing. you can demonstrate your model by running the model created with extension `.pt`.

## Dataset
The dataset used for this project includes various images of recyclable and non-recyclable items like cardboard, glass, clothes etc. annotated for object detection and segmentation. The dataset is preprocessed using AutoDistill and GroundedSAM.

## Model Training
The model is trained using the YOLOv8 architecture. The training process involves:
- Loading the dataset
- Data augmentation
- Model training
- Evaluation

## Real-time Testing
Real-time testing is facilitated through OpenCV2, allowing the model to detect and classify waste items using a webcam.

## Results
The model achieves high accuracy in detecting and classifying waste items, demonstrating its effectiveness in real-world scenarios.

## Acknowledgements
- **Ultralytics** for the YOLOv8 model
- **AutoDistill** and **GroundedSAM** for image segmentation and annotation tools
- **Google Colab** for providing the computational resources
