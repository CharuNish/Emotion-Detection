# Facial Keypoint Detection

## Introduction
This project aims to develop a deep learning model capable of detecting 15 facial keypoints to analyze customer emotions and facial expressions effectively. Utilizing the power of Convolutional Neural Networks (CNN) and Residual Blocks, the model is built with Keras using TensorFlow 2.0 as the backend. This approach enables the precise identification of facial features, which can be pivotal in various applications, including emotion detection, augmented reality, and more.

## Dataset Description
The dataset for this project consists of images and corresponding facial keypoint data. Each keypoint is defined by an (x, y) pair representing its pixel index position within a 96x96 pixel image. The keypoints cover critical facial features, including:

- Left and right eye centers
- Inner and outer corners of both eyes
- Inner and outer ends of both eyebrows
- Nose tip
- Left and right corners of the mouth
- Center top and bottom lip

The "left" and "right" designations refer to the subject's perspective. Each image is accompanied by a list of pixels, represented as integers ranging from 0 to 255, which describe the facial features.

## Model Description
The model is built using an architecture that combines Convolutional Neural Networks (CNN) with Residual Blocks. This design choice was motivated by the need to capture complex facial structures accurately while avoiding the vanishing gradients problem often encountered in deep learning models.

### Key Features:
- **Framework**: Keras with TensorFlow 2.0 backend
- **Architecture**: Custom CNN with Residual Blocks
- **Objective**: Detect 15 distinct facial keypoints
- **Input**: 96x96 pixel grayscale images
- **Output**: (x, y) coordinates for each of the 15 facial keypoints

## Training
The model was trained over 100 epochs, utilizing a dataset split into training and validation sets to ensure robustness and generalizability. During training, various techniques such as data augmentation and dropout were employed to prevent overfitting.

## Results
After training, the model achieved an accuracy of 85.98%, demonstrating its effectiveness in detecting facial keypoints with high precision. 

