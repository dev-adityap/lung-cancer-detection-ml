# Lung Cancer Detection Using Machine Learning

A supervised machine learning project for detecting the presence or absence of lung cancer using patient survey and clinical risk-factor data.

## 📌 Project Overview

This project applies supervised machine learning classification techniques to predict whether a patient is likely to have lung cancer based on clinical attributes and associated risk factors.

Three classification algorithms were implemented and compared:

- Logistic Regression
- Decision Tree
- Random Forest

The models were trained and evaluated using the same dataset and test set to provide a fair comparison.

---

## 🎯 Problem Statement

Lung cancer detection can benefit from analyzing patient-related risk factors and symptoms.

The objective of this project is to build a binary classification system that predicts:

- **1 → Lung Cancer Detected**
- **0 → No Lung Cancer Detected**

---

## 📊 Dataset

The project uses the **Lung Cancer Survey Dataset**, containing:

- **309 patient records**
- **15 input features**
- **1 target variable**
- **2 target classes**
- No missing values

The dataset contains patient attributes and risk factors such as:

- Gender
- Age
- Smoking
- Yellow Fingers
- Anxiety
- Peer Pressure
- Chronic Disease
- Fatigue
- Allergy
- Wheezing
- Alcohol Consuming
- Coughing
- Shortness of Breath
- Swallowing Difficulty
- Chest Pain

### Target Variable

`LUNG_CANCER`

| Original Value | Encoded Value |
|---|---:|
| YES | 1 |
| NO | 0 |

---

## 🔄 Data Preprocessing

The following preprocessing steps were performed:

1. Dataset was loaded using Pandas.
2. Input features and target variable were separated.
3. Categorical values were converted into numerical values.
4. `GENDER` was encoded as:
   - M → 1
   - F → 0
5. Binary features were represented numerically.
6. The final dataset was converted into numerical form suitable for machine learning models.

---

## 📈 Exploratory Data Analysis

A correlation heatmap was generated to analyze relationships between the dataset features and the target variable.

### Correlation Heatmap

![Correlation Heatmap](images/correlationheatmap.png)

---

## 🧠 Model Architecture

The project follows the following machine learning pipeline:

```text
Patient Dataset
       ↓
Data Preprocessing
       ↓
Feature Encoding
       ↓
Train-Test Split
       ↓
 ┌───────────────┬───────────────┬───────────────┐
 ↓               ↓               ↓
Logistic       Decision        Random
Regression      Tree           Forest
 ↓               ↓               ↓
 └───────────────┴───────────────┘
                 ↓
          Model Evaluation
                 ↓
      Accuracy / Precision /
       Recall / F1 Score
                 ↓
       Final Model Selection
