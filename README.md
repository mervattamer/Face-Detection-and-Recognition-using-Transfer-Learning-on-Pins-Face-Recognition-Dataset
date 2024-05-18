# Face Recognition and Detection using Transfer Learning

This project aims to implement face detection and recognition using transfer learning techniques. The dataset used for training and testing the models can be found [here](https://www.kaggle.com/datasets/hereisburak/pins-face-recognition).

## Table of Contents
1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Face Detection](#face-detection)
4. [Dataset Preprocessing](#dataset-preprocessing)
5. [Face Recognition](#face-recognition)
6. [Model Enhancement](#model-enhancement)
7. [Non-Classified Face Recognition](#non-classified-face-recognition)
8. [Live Camera Implementation](#live-camera-implementation)
9. [Conclusion](#conclusion)
10. [License](#license)

## Introduction
This project utilizes transfer learning techniques to perform face detection and recognition tasks. It combines OpenCV's deep learning face detector and Inception V3 model for face recognition.

## Setup
1. Clone this repository.
2. Install the required dependencies listed in `requirements.txt`.

## Face Detection
The deep learning face detector provided by OpenCV is used for face detection. It is based on the "Face detector (UINT8)" model.

## Dataset Preprocessing
The dataset is preprocessed by cropping faces using OpenCV DNN module. This results in a modified dataset suitable for training face recognition models.

## Face Recognition
Inception V3 model, pretrained on ImageNet, is used as a transfer learning model for face recognition. You can download the pretrained weights from [here](https://github.com/fchollet/deep-learning-models/releases/download/v0.5/inception_v3_weights_tf_dim_ordering_tf_kernels.h5).

## Model Enhancement
Dense layers and softmax layers are added after the transfer learning phase to enhance the model's accuracy.

## Non-Classified Face Recognition
The model is trained to recognize non-classified faces using cosine similarity. A class of 70K non-mentioned photos named "non-defined" is created for this purpose.

## Live Camera Implementation
The model runs on a live camera feed, performing both face detection and recognition simultaneously (SIMO model).

## Conclusion
This project provides a comprehensive solution for face recognition and detection using transfer learning techniques. It is suitable for both academic research and practical applications.
