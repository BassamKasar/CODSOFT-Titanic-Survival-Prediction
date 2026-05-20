# Titanic Survival Prediction - CodSoft Task 1

This repository contains the code and documentation for the **Titanic Survival Prediction** project, completed as part of my Data Science internship at **CodSoft**.

---

## Project Overview

The goal of this project is to build a machine learning model that predicts whether a passenger on the Titanic survived or not based on various features such as age, gender, ticket class, and fare.

This is a classic **binary classification problem**, where the target variable is `Survived`:
- **1** = Survived
- **0** = Deceased

---

## Dataset

The project utilizes the `Titanic-Dataset.csv` file, which includes:

| Feature     | Description                                      |
|-------------|--------------------------------------------------|
| Pclass      | Ticket class (1st, 2nd, or 3rd)                 |
| Sex         | Gender of the passenger                         |
| Age         | Age in years                                    |
| SibSp       | Number of siblings/spouses aboard               |
| Parch       | Number of parents/children aboard               |
| Fare        | Ticket price                                    |
| Embarked    | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## Workflow

### 1. Data Loading
- Read the dataset using **Pandas**.

### 2. Data Cleaning
- Handled missing values for `Age` using the **median**.
- Filled missing `Embarked` values with the **mode**.
- Dropped irrelevant columns (`Name`, `Ticket`, `Cabin`, `PassengerId`).

### 3. Feature Encoding
- Converted categorical text data into numerical values using **LabelEncoder**.

### 4. Model Training
- Trained a **Random Forest Classifier** to identify patterns in the data.

### 5. Evaluation
- Validated the model using **accuracy scores** and a **classification report**.

---

## Results

| Metric            | Score     |
|-------------------|-----------|
| Model Accuracy    | **~81.5%** |

### 🔍 Key Insight
- **Gender (Sex)** was the most significant predictor of survival, followed by the passenger's fare and class.
