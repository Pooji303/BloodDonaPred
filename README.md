# 🩸 Blood Donation Prediction

This project applies machine learning techniques to predict blood donation behavior based on historical donation records. It involves data preprocessing, feature engineering, model training, and evaluation.

## 📌 Project Overview

Blood donation is a critical aspect of healthcare, ensuring a stable supply for medical needs. This project aims to predict whether a donor will donate blood in the future, helping blood banks optimize their donor outreach and inventory management.

## 📂 Directory Structure

```
├── data
│   ├── raw/         # Original dataset
│   ├── processed/   # Cleaned and transformed data
│  
├── notebooks
│   ├── EDA.ipynb              # Exploratory Data Analysis
│   ├── feature_engineering.ipynb  # Feature selection and engineering
│   ├── model_training.ipynb   # Model selection and training
│   ├── model_evaluation.ipynb # Performance evaluation
│  
├── src
│   ├── preprocessing.py  # Data preprocessing functions
│   ├── train.py          # Model training script
│   ├── predict.py        # Prediction script
│  
├── reports
│   ├── results.md        # Analysis and model evaluation results
│  
└── README.md             # Project Documentation
```

## 🚀 Technologies Used

- **Python**
- **Scikit-learn**
- **Logistic Regression**
- **SMOTE (Synthetic Minority Over-sampling Technique)**
- **Seaborn & Matplotlib (for visualization)**

## 📊 Data Processing

- Standard scaling applied to normalize features.
- SMOTE used to handle class imbalance.
- Features selected based on exploratory data analysis.

## 🔍 Model Training

- **Model:** Logistic Regression
- **Hyperparameter tuning** performed using GridSearchCV.
- **Performance metrics:** Accuracy, Precision, Recall, F1-score, Confusion Matrix.

## 📝 Results & Insights

- **Data Cleaning:**  
  - Outliers were removed using the **Interquartile Range (IQR) method** for features such as:
    - Resting blood pressure  
    - Serum cholesterol  
    - Oldpeak (ST depression)  
    - Age  
    - Maximum heart rate achieved  
  - Removing extreme values instead of replacing them helped maintain data integrity and reduced overfitting risk.

- **Feature Engineering:**  
  - The most influential categorical features include:
    - **Slope of peak exercise ST segment**
    - **Chest pain type**
    - **Number of major vessels**
    - **Fasting blood sugar level**
    - **Resting ECG results**
    - **Sex**
    - **Exercise-induced angina**

- **Model Performance:**  
  - The model was evaluated using standard metrics:
    - **Accuracy**
    - **Precision**
    - **Recall**
    - **F1-score**
    - **Confusion Matrix**
  - Hyperparameter tuning was performed using **GridSearchCV** to improve performance.

