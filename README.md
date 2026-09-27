# Diabetes Prediction Using Machine Learning

A machine learning project that predicts whether a person is likely to have diabetes based on medical diagnostic measurements.

## Project Overview

This project uses the **Pima Indians Diabetes Dataset** to build and evaluate multiple machine learning classification models.

The project compares different algorithms and selects **Linear Support Vector Machine (SVM)** as the final model based on the model evaluation performed.

The system takes medical measurements such as glucose level, blood pressure, BMI, age, and other diagnostic information as input and predicts whether the person is diabetic or not.

## Dataset

The dataset contains **768 records** and **8 input features**.

### Features

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

### Target

- `Outcome = 0` → Not Diabetic
- `Outcome = 1` → Diabetic

## Machine Learning Models Compared

The following classification algorithms were evaluated:

- Logistic Regression
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Naive Bayes

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- 5-Fold Stratified Cross-Validation

## Final Model

The final model selected for the project is:

**Linear Support Vector Machine (SVM)**

The input features are standardized using `StandardScaler` before prediction.

### Final Test Performance

- Accuracy: **77.27%**
- Precision: **75.68%**
- Recall: **51.85%**
- F1-Score: **61.54%**

The model's performance was evaluated on a separate test set.

## Prediction

The project includes a prediction function that accepts the following inputs:

```text
Pregnancies
Glucose
BloodPressure
SkinThickness
Insulin
BMI
DiabetesPedigreeFunction
Age