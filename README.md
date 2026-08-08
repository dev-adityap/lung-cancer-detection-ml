# Lung Cancer Detection Using Machine Learning

A supervised machine learning project for detecting the presence or absence of lung cancer using patient survey and clinical features.

## 📌 Project Overview

This project develops a binary classification system that predicts whether a patient is likely to have lung cancer based on 15 clinical and lifestyle-related features.

Three machine learning classification algorithms were trained and evaluated:

- Logistic Regression
- Decision Tree
- Random Forest

Random Forest was selected as the final model because it achieved the highest tied accuracy along with strong precision, recall, and F1-score, while also providing feature importance analysis.

## 📊 Dataset

- Total records: **309**
- Input features: **15**
- Target classes: **2**
- Training records: **247**
- Testing records: **62**
- Train-test split: **80:20**

The target variable is `LUNG_CANCER`.

```text
YES → 1
NO  → 0
