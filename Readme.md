# 🩺 Breast Cancer Classification Using Machine Learning

## 📋 Introduction

Breast cancer is one of the most common cancers affecting women globally. Early detection is crucial for improving survival rates, but traditional diagnostic methods often rely on subjective visual inspections by doctors, which can lead to errors due to human limitations. Studies have shown that machine learning can significantly improve the accuracy of breast cancer diagnosis, surpassing even the most experienced physicians in some cases. This project aims to build a robust machine learning model to assist in classifying breast tumors as **benign** or **malignant**, improving diagnostic accuracy and reducing the reliance on manual interpretation.

## 🎯 Objective

The main goal of this project is to implement a machine learning-based diagnostic tool for classifying breast cancer tumors, helping doctors make better, faster, and more reliable decisions.

### Why Machine Learning for Breast Cancer Diagnosis?

- **Improved Accuracy**: Studies show that machine learning can improve diagnostic accuracy, achieving up to 91.1% correct diagnoses compared to 79.97% by experienced physicians.
- **Pattern Recognition**: Machine learning models can quickly and accurately detect patterns that are not easily identifiable by humans.
- **Assistive Tools**: These models serve as computer-aided diagnostic tools, assisting physicians by providing a second, more objective opinion.

## 🔍 Problem Overview

Breast tumors are broadly classified into two types:
- **Benign**: Non-cancerous, but can increase the risk of developing breast cancer later.
- **Malignant**: Cancerous and often more dangerous. Approximately 20% of women diagnosed with malignant tumors succumb to the disease.

Given the importance of early and accurate diagnosis, this project employs machine learning techniques to classify tumors as benign or malignant, thereby contributing to better patient outcomes.


## 🛠️ Approach

In this project, we use a **Logistic Regression** model to classify breast tumors as **benign** or **malignant**. Logistic Regression is a powerful yet simple algorithm that works well for binary classification problems like this one. It provides interpretable results and performs efficiently even on relatively small datasets.

### Key Steps:
1. **Data Preprocessing**: 
   - We clean the data, handle missing values, and normalize features for better model performance.
   - We also split the data into **training** and **test** sets to evaluate the model's performance on unseen data.
  
2. **Model Building**: 
   - We implemented a **Logistic Regression** model using **Scikit-learn** to classify tumors based on their characteristics.
   - To improve accuracy, we experimented with feature selection to remove irrelevant components and reduce dimensionality, preventing overfitting.

3. **Evaluation**: 
   - We evaluated the model using common metrics such as **accuracy** on both the training and test datasets.

### Performance:
- **Accuracy on training data**: 94.73%
- **Accuracy on test data**: 92.98%

The high accuracy on both training and test data indicates that the model generalizes well to unseen data, making it a reliable tool for classifying breast cancer tumors.

## 📊 Dataset

I used the **Breast Cancer Wisconsin (Diagnostic) Dataset** from [Kaggle](https://www.kaggle.com/c/breast-cancer-classification), which includes various features describing the characteristics of cell nuclei in breast cancer patients. These features serve as the basis for tumor classification.

### Key Features:
- **Mean radius, texture, perimeter, area, and smoothness** of tumors.
- **Class labels**: 0 (Benign), 1 (Malignant).
