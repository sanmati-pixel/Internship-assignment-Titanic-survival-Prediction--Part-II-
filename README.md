# Internship-assignment-Titanic-survival-Prediction--Part-II-
# Titanic Survival Prediction 🚢

This project predicts passenger survival on the Titanic using machine learning techniques.  
It was developed as part of my internship work and submitted to the Kaggle Titanic competition.

---

## 📌 Project Overview
The goal of this project is to analyze the Titanic dataset, perform data preprocessing and feature selection, and build predictive models to determine whether a passenger survived or not.

The complete machine learning workflow was followed:
- Data understanding & exploration
- Data preprocessing
- Feature selection
- Model training & comparison
- Kaggle submission

---

## 📊 Data Understanding & Exploration (EDA)
- Analyzed passenger demographics such as:
  - Gender distribution
  - Passenger class
  - Cabin availability
- Studied survival rates based on:
  - Passenger class
  - Gender
  - Boarding location
  - Cabin vs non-cabin passengers
- Explored relationships between features and survival outcomes

---

## 🧹 Data Preprocessing
- Identified missing values and handled them appropriately:
  - **Age** → median imputation
  - **Embarked** → mode
  - **Fare** → mode
- Created meaningful derived features to improve model learning
- Prepared the dataset for feature selection and model training

> 🔎 Detailed categorical encoding is handled separately and documented in its own module.

---

## 🔧 Feature Selection
Used **Recursive Feature Elimination (RFE)** to identify the most important features contributing to survival prediction.

Selected features include:
```python
['Pclass', 'SibSp', 'Parch', 'Fare', 'isCabin', 'female', 'C', 'Q', 'S']
