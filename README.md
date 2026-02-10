# Exploring-Convolutional-Layers-Through-Data-and-Experiments


## PROBLEM:

Pneumonia is an important and critical respiratory infection. If pneumonia infection is not timely detected, it could be life-threatening. Radiologists normally rely on images from a chest X-ray to identify any pneumonia symptoms. Nevertheless, the task of performing this function is cumbersome and sometimes prone to human error.

The goal of this project is to build a machine learning system that can learn to classify chest X-ray images automatically into either Normal or Pneumonia. By using deep learning techniques, this system can assist medical experts by providing a quick and accurate diagnostic system.

The dataset used for this model contains labeled chest X-ray images of pediatric patients, which enables learning by patterns related to pneumonia infection.

## Description of the dataset:

The Chest X-Ray Pneumonia dataset used in the project consists of chest radiographic images and is divided into two classes: Normal and Pneumonia. These images were collected from pediatric patients, and this dataset is rather common for research in medical image classification.

The dataset has been divided into three parts: training, validation, and testing. Each of the subsets contains images stored in class-specific folders, which may allow for automatic labeling during data loading. There is a large difference in size between the training set and both the validation and test sets, enabling the model to learn patterns relevant to pneumonia.

The images differ in both resolution and color channels, with the majority of them being grayscale chest X-rays. Each of these images was resized to a certain fixed dimension for consistency in training and then normalized. This is a binary classification problem where the goal is to classify lungs as healthy or affected by pneumonia.

## Experimental results:

| Model Depth   | Validation Accuracy | Validation Loss |
| ------------- | ------------------- | --------------- |
| 1 Conv Layer  | 0.9375              | 0.1810          |
| 2 Conv Layers | 0.9375              | 0.1297          |
| 3 Conv Layers | 0.8125              | 0.3837          |

## Interpretations:

However, the model with two convolutional layers scored the best overall based on the results. While the one-layer model was comparable with regard to accuracy, the higher loss suggests that predictions were less confident. Moving to the three-layer model, there was a decline in overall model performance. This was expected due to overfitting or inadequate data for the model.

These results show that it’s not necessarily true that a more complex model will perform better, proving that an intermediate depth gave the best balance between feature extraction capacity and overall model generalization.