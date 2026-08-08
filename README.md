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
🧹 Data Preprocessing

The dataset was prepared before model training.

Categorical values were converted into numerical form.
GENDER was encoded as:
M → 1
F → 0
LUNG_CANCER was encoded as:
YES → 1
NO → 0
Binary features were represented numerically.
The final dataset contained numerical features suitable for machine learning.
🔬 Exploratory Data Analysis

Exploratory analysis was performed to understand the dataset and relationships between variables.

The project includes:

Dataset inspection
Feature analysis
Correlation heatmap
Random Forest feature importance
Model performance visualization
🤖 Machine Learning Models
1. Logistic Regression

Used as a baseline classification model for binary prediction.

2. Decision Tree

A tree-based classification model capable of learning non-linear decision boundaries.

3. Random Forest

An ensemble learning algorithm that combines multiple decision trees to improve robustness and generalization.

📈 Model Performance
Model	Accuracy	Precision	Recall	F1 Score
Logistic Regression	96.77%	98.33%	98.33%	98.33%
Decision Tree	95.16%	98.31%	96.67%	97.48%
Random Forest	96.77%	98.33%	98.33%	98.33%
🏆 Final Model

Random Forest Classifier

Random Forest was selected as the final model because:

It achieved a tied highest accuracy of 96.77%.
It achieved strong precision, recall, and F1-score.
It uses an ensemble of multiple decision trees.
It provides feature importance analysis.
It can capture feature interactions effectively.
📊 Evaluation

The models were evaluated using:

Accuracy
Precision
Recall
F1 Score
Confusion Matrix

The test set contained 62 records.

Random Forest correctly classified 60 out of 62 test samples.

🧠 Feature Importance

Random Forest feature importance was used to identify which features contributed most to the model's predictions.

In the trained model, AGE had the highest feature importance, followed by features including:

Alcohol Consuming
Allergy
Peer Pressure
Yellow Fingers
Fatigue
Coughing
🛠️ Technologies Used
Python
Google Colab
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
📁 Project Structure
lung-cancer-detection-ml/
│
├── Lung_Cancer_Detection_ML.ipynb
├── LUNG CANCER DETECTION PBL ML 251.docx
└── README.md
▶️ How to Run
Download or clone this repository.
Open Lung_Cancer_Detection_ML.ipynb in Google Colab or Jupyter Notebook.
Upload the required dataset.
Run the notebook cells sequentially.
Review the model evaluation results and visualizations.
🔮 Future Improvements

Possible improvements include:

Handling class imbalance using appropriate resampling techniques.
Hyperparameter tuning.
Cross-validation.
Testing additional machine learning algorithms.
Developing a web-based prediction interface.
Evaluating the model on a larger and more diverse dataset.
⚠️ Disclaimer

This project is intended for educational and research purposes only. The predictions produced by the model should not be considered a medical diagnosis or a substitute for professional medical advice.
