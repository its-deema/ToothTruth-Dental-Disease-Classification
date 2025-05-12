# 🦷 Advanced Deep Learning Models for Classifying Dental Diseases from Panoramic Radiographs

This repository contains the implementation of our Graduation Project:Dental disease classification system using deep learning models on panoramic radiographs. Our project aims to provide accurate and efficient classification of various dental conditions to assist dental professionals in diagnosis.

## 👩‍💻 Team Members
- [@ReemaAlnasser](https://github.com/byReema)
- [@WareefAlolayan](https://github.com/WareefAlolayan)
- [@ShihanahAlbadi](https://github.com/Shihanaah)
- [@DeemaAlnasser](https://github.com/its-deema)

## 📝 Project Overview

We conducted a comprehensive comparison of various deep learning models for multiclass classification of dental problems using panoramic radiographs. Our results demonstrate the effectiveness of models like EfficientNetV2 and DenseNet-121 in accurately identifying multiple dental conditions from a single radiographic image.

## 🗂️ Dataset

- **Original Dataset**: The project uses the vzrad2 dataset containing 10,580 panoramic radiographs across 93 different dental disease classes. The original dataset can be accessed via Roboflow: [vzrad2 Dataset](https://universe.roboflow.com/arshs-workspace-radio/vzrad2)

- **Processed Dataset**: We refined the original dataset by:
  - Consolidating semantically equivalent terms (e.g., "Caries" and "Cavity")
  - Correcting misspellings and inconsistencies
  - Implementing a hierarchical classification structure
  - Reducing the number of classes from 93 to 35 distinct classes organized under 22 parent categories
  - Applying targeted augmentation to address class imbalance (reducing imbalance ratio from 2560:1 to 61:1)

The processed dataset is available in the `Final_processed_dataset` folder within this repository.

## 🧠 Models Implemented

We implemented and compared five state-of-the-art deep learning architectures:

1. **EfficientNetV2** - Achieved 97.04% accuracy and 95.79% mAP
2. **DenseNet-121** - Achieved 96.70% accuracy and 94.25% mAP
3. **ResNet50** - Achieved 95.45% accuracy and 91.29% mAP
4. **VGG16** - Achieved 95.40% accuracy and 93.20% mAP
5. **InceptionV3** - Achieved 94.49% accuracy and 89.14% mAP

## 📈 Implementation

The project implementation includes:

- Data preprocessing and augmentation pipeline
- Model-specific fine-tuning strategies
- Focal Loss implementation to address class imbalance
- Comprehensive evaluation using multiple metrics (accuracy, precision, recall, F1-score, mAP)

## 📊 Results

Our findings indicate that EfficientNetV2 is the most effective architecture for dental disease classification, achieving an accuracy of 97.04% and mAP of 95.79%. The model demonstrates strong performance across various dental conditions, including orthodontic brackets, caries, decay, and fillings.

## 📸 Sample Output

### Dataset Structure
After restructuring the classes, we organized dental conditions into a hierarchical structure as shown below:

<img width="881" alt="Dental Diseases Tree" src="https://github.com/user-attachments/assets/fb4e57c3-06bb-4e8a-984f-5e19f99f610c" />


### Model Predictions
Below is a sample visualization showing ground truth annotations (left) and model predictions (right):

![DensNet121_prediction_comparison](https://github.com/user-attachments/assets/85588770-489b-4da5-8874-bc05ed2044da)
