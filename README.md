# Skin Lesion Classification using CNNs

## Overview
This project focuses on **multiclass skin lesion classification** using **convolutional neural networks (CNNs)** applied to dermoscopic images from the **ISIC 2018 Skin Cancer dataset**.  
The work explores baseline CNN modeling, strategies for handling **highly imbalanced medical data**, model performance improvements, and **transfer learning** with pretrained architectures.

---

## Problem Description
Skin lesion classification is a challenging computer vision task with significant real-world impact in early skin cancer detection.  
The objective of this project is to design and evaluate deep learning models that can accurately classify skin lesions across multiple categories while addressing common issues such as **class imbalance** and limited data for minority classes.

---

## Dataset
- **Source:** International Skin Imaging Collaboration (ISIC 2018)
- **Data type:** Dermoscopic RGB images
- **Task:** Multiclass image classification (7 classes)

### Key Characteristics
- Highly imbalanced class distribution  
- Majority of samples belong to the *Melanocytic nevi* class  
- Minority classes are underrepresented, increasing classification difficulty

---

## Exploratory Data Analysis
Exploratory analysis was performed to:
- Visualize random image samples and labels
- Analyze class distribution
- Identify dataset imbalance and potential biases

The analysis revealed a **severely imbalanced dataset**, motivating the use of targeted mitigation strategies during model training.

---

## Methodology

### Baseline CNN
- Custom CNN architecture with convolutional, pooling, and dense layers
- Trained using Adam optimizer and cross-entropy loss
- Performance evaluated on validation and test sets

### Handling Class Imbalance
To improve minority-class performance, multiple techniques were explored:
- **Data augmentation** to increase sample diversity
- **Class weighting** to penalize misclassification of underrepresented classes
- **Undersampling** of the dominant class

The impact of each strategy was analyzed using class-level metrics.

### Model Improvement
- Architectural modifications and hyperparameter tuning
- Comparison against the baseline CNN

### Transfer Learning
- Pretrained CNNs (VGG16) used as feature extractors
- Frozen convolutional layers with custom classification heads
- Performance compared against baseline and fine-tuned CNNs

---

## 📈 Evaluation & Results
Models were evaluated using:
- Accuracy
- Sensitivity & Specificity
- F1-score
- ROC curves with AUC
- Confusion matrices

### Key Findings
- Class imbalance significantly affects naive CNN performance
- Imbalance mitigation improves minority-class sensitivity and F1-score
- Transfer learning achieves the strongest overall performance
- Accuracy alone is insufficient for evaluating imbalanced medical datasets


## Project Context
This project was completed as part of a **group university assignment**.  
This repository contains the **notebook reflecting my individual implementation, experimentation, and analysis**.  
The final written report was completed individually.


