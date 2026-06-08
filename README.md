# ML-project
# Titanic Survival Prediction

## Overview

This project uses the Titanic dataset to predict whether a passenger survived or not. Several machine learning models and a neural network were trained and compared to identify the best-performing approach.

## Dataset

The dataset contains information about Titanic passengers. The target variable is:

* **Survived** (0 = Did Not Survive, 1 = Survived)

Features used:

* PassengerId
* Pclass
* SibSp
* Parch
* Fare

The dataset contains 891 records.

## Models Used

### 1. K-Nearest Neighbors (KNN)

* Accuracy: 67.60%
* F1-Score: 0.517

### 2. Logistic Regression

* Accuracy: 71.51%
* F1-Score: 0.587

### 3. Random Forest

* Accuracy: 65.36%
* F1-Score: 0.544

### 4. Neural Network (Keras)

Architecture:

* Dense (16 neurons, ReLU)
* Dropout (0.2)
* Dense (8 neurons, ReLU)
* Dropout (0.2)
* Dense (1 neuron, Sigmoid)

Training:

* Optimizer: Adam
* Loss Function: Binary Crossentropy
* Epochs: 20

Results:

* Accuracy: 72.63%
* F1-Score: 0.602

## Results Summary

| Model               | Accuracy | F1-Score |
| ------------------- | -------- | -------- |
| KNN                 | 0.676    | 0.517    |
| Logistic Regression | 0.715    | 0.587    |
| Random Forest       | 0.654    | 0.544    |
| Neural Network      | 0.726    | 0.602    |

The Neural Network achieved the highest Accuracy and F1-Score, making it the best-performing model in this project.

## Key Learnings

* Data preprocessing has a significant impact on model performance.
* Different machine learning models can produce very different results on the same dataset.
* Neural Networks can outperform traditional machine learning models, even with a simple architecture.
* F1-Score is useful when classes are not perfectly balanced.

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib

## Author

Created as part of a Machine Learning coursework project.
