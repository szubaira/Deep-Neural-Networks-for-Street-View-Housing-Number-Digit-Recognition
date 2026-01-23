# SVHN Digit Recognition Using Deep Learning

## Overview

The goal of this project was to build and evaluate a deep learning model capable of accurately recognizing digits from real-world images using the Street View House Numbers (SVHN) dataset. The project leveraged convolutional neural networks (CNNs) to classify digits (0–9) appearing in natural scenes, such as house numbers captured by Google Street View.

The final deep learning model achieved strong classification performance on unseen test data, demonstrating the effectiveness of CNN architectures for image recognition tasks. Through model training and evaluation, key architectural and training parameters contributing to improved accuracy were identified.

## Business Understanding

Digit recognition from real-world images has widespread applications, including automated address reading, postal mail sorting, document digitization, and intelligent transportation systems. Unlike handwritten digit datasets, real-world images contain noise, lighting variations, and background clutter, making accurate classification more challenging.

The objective of this project was to design a robust deep learning solution that can reliably recognize digits under these realistic conditions, helping businesses automate processes that depend on accurate numeric information extraction.

## Data Understanding 

The SVHN dataset consists of labeled images of digits (0–9) extracted from street-level imagery. Each image contains a single digit with variations in scale, color, orientation, and background. The dataset includes separate training and testing sets, allowing for proper model evaluation.

Initial exploration focused on understanding image dimensions, label distribution, and pixel value ranges. Images were normalized and reshaped to ensure compatibility with convolutional neural network architectures.

Link to data: https://drive.google.com/file/d/1YoTWTdShWdI55SmBp4Ie2IkaI_E3Gmp0/view?usp=sharing

<img width="792" height="119" alt="Screen Shot 2026-01-23 at 01 06 17" src="https://github.com/user-attachments/assets/431ca346-c666-47e2-8b55-a3fcf8d3920d" />

## Data Preparation

**Data preprocessing steps included:**

- Normalizing pixel values to improve model convergence

- Reshaping image arrays to match CNN input requirements

- Encoding digit labels into categorical format

- Splitting data into training and validation subsets

These steps ensured that the dataset was clean, standardized, and ready for deep learning model training.

## Modeling and Evaluation

A convolutional neural network (CNN) was implemented using a deep learning framework to learn spatial patterns in digit images. The model architecture included convolutional layers, pooling layers, and fully connected layers to extract and classify visual features.

Model performance was evaluated using accuracy metrics on validation (76%)and test (78%) datasets. The trained model demonstrated strong generalization ability, accurately recognizing digits across a wide range of image conditions. Performance improvements (increased to 80% f1 score) were achieved through tuning hyperparameters such as learning rate, batch size, and network depth.

<img width="791" height="772" alt="Screen Shot 2026-01-23 at 01 05 38" src="https://github.com/user-attachments/assets/7e612f7f-e2da-4936-96d8-9e1b2c77a76f" />
<img width="785" height="536" alt="Screen Shot 2026-01-23 at 01 06 47" src="https://github.com/user-attachments/assets/b5de8351-dc95-4617-933b-38b0bb0cabc4" />

## Conclusion

This project demonstrates the effectiveness of deep learning techniques for real-world image classification tasks. The CNN model successfully learned to recognize digits from complex visual environments, highlighting its potential for deployment in practical applications such as automated data entry and visual recognition systems.

Future enhancements could include experimenting with deeper architectures, applying data augmentation techniques, or extending the model to multi-digit recognition scenarios.
