<div style="text-align:center">
    <img src="https://github.com/OmarGaafar1/Instant-Smile-Detection/assets/92587188/42f633bb-7eb0-4bcb-a8c9-d1f8a9e4007f" alt="child_result">
</div>

# Smile Detection Model README

## Overview

This project involves the creation of a smile detection model using convolutional neural networks (CNNs). The model is trained to automatically detect whether a person in an image or video frame is smiling or not. The model is implemented using TensorFlow and Keras libraries.

## Model Description

The smile detection model is a supervised CNN model. It is trained on a dataset of labeled images where each image is categorized as either "smiling" or "not smiling". During training, the model learns to extract features from the input images and classify them into the appropriate categories based on these features. The model's parameters are optimized using supervised learning techniques to minimize the classification error, enabling it to accurately identify smiles in real-world scenarios.

## Program Functionality

The smile detection program captures face images from a video feed using OpenCV and sends them to the trained smile detection model for inference. Here's an overview of the program's functionality:

1. **Capture Face Images:** 
   - Utilizes OpenCV to capture frames from a video feed.
   - Detects faces in each frame using a face detection algorithm.
   - Extracts face regions from the frames containing detected faces.

2. **Preprocess Images:** 
   - Preprocesses the extracted face images (resize, normalize, etc.) to prepare them for input to the smile detection model.

3. **Send Images to Model:** 
   - Passes the preprocessed face images to the trained smile detection model for inference.
   - The model predicts whether each face is smiling or not.

4. **Display Results:** 
   - Overlays the smile prediction (smiling or not smiling) on the original video frames.
   - Displays the updated video feed with smile predictions in real-time.

## Project Files

- `Convolution Neural Network Classifier.ipynb`: This notebook contains the implementation of the smile detection model, including data preprocessing, model training, evaluation, and saving the trained model.
- `Main.ipynb`: This notebook contains the main function which starts the video capturing and sends and receives inputs from the model.
- `data/`: This directory contains the trained data.
- `README.md`: This README file provides an overview of the project, including the model description, program functionality, and project files.
- `requirements.txt`: This file lists all the Python libraries required by the project. Use `pip install -r requirements.txt` to install the dependencies.
- `Completed Model/`: This folder contains the pre-trained model that is ready for production.
  

## Getting Started

To run the smile detection program, follow these steps:

1. Clone the project repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Open the `Main.ipynb` notebook and run it to start the video capturing and smile detection process.


