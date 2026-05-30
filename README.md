# skin-cancer-detection-deep-learning

Deep learning-based skin cancer classification using CNN and ResNet50 on the HAM10000 dataset.

---

## Overview

This project focuses on multi-class skin lesion classification using deep learning and computer vision techniques. The goal is to classify skin cancer images into different categories using both a custom CNN model and transfer learning with ResNet50.

The project explores the complete machine learning workflow, including preprocessing, augmentation, model training, fine-tuning, and performance evaluation.

---

## Dataset

**Dataset:** HAM10000 (Human Against Machine with 10000 Training Images)

* Total images: ~10,000 dermatoscopic skin lesion images
* Number of classes: **7 skin lesion categories**
* Source: Kaggle HAM10000 Dataset

The dataset was split into **train, validation, and test sets using stratified sampling** to maintain class balance.

---

## Features

* Image preprocessing and normalization
* Data augmentation for better generalization
* Stratified train-validation-test split
* Custom CNN model implementation
* Transfer learning using **ResNet50**
* Fine-tuning pretrained model layers
* Class imbalance handling using class weights
* Performance evaluation using:

  * Accuracy
  * Precision
  * Recall
  * F1-score
  * Confusion Matrix

---

## Model Architecture

### 1. Custom CNN

A convolutional neural network built using TensorFlow/Keras consisting of:

* Multiple convolutional layers
* Max pooling
* Dense layers
* Dropout regularization

### 2. ResNet50 Transfer Learning

A pretrained **ResNet50** model was used with:

* Frozen base layers initially
* Custom classification head
* Fine-tuning of later layers
* Learning rate scheduling and early stopping

---

## Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn

---

## Workflow

1. Dataset download and preprocessing
2. Data augmentation
3. Custom CNN training
4. ResNet50 transfer learning
5. Fine-tuning model layers
6. Performance evaluation on test data
7. Visualization using confusion matrix and training curves

---

## Results

* Achieved approximately **85.7% test accuracy** using transfer learning with ResNet50.
* Performance evaluated using classification metrics and confusion matrices.

---

## Project Structure

```bash
skin-cancer-detection-deep-learning/
│── README.md
│── requirements.txt
│── skin_cancer_detection.ipynb
│── Results/
│   ├── CNN_Accuracy_graph.png
│   ├── CNN_Confusion_Matrix.png
│   ├── ResNet50_Confusion_Matrix.png
```

## Future Improvements

* Experiment with EfficientNet and Vision Transformers
* Add Grad-CAM visualization for explainability
* Deploy using Flask or Streamlit
* Improve classification performance through hyperparameter tuning

---

## Author

**Shivanshu Pauskar**

GitHub: https://github.com/ShivanshuPauskar
