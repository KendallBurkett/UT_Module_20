## Supervised Learning
---

# Credit Risk Classification

## Table of Contents
- [Description](#description)
- [Data Files](#data-files)
- [Features](#features)
- [Installation](#installation)
- [Results](#results)
- [Overview of the Analysis](#overview-of-the-analysis)
- [Summary](#summary)
- [Author](#author)

---

## Description

The **Credit Risk Classification** project uses supervised machine learning techniques to analyze credit risk data and predict whether a loan is high risk or low risk. This project leverages **logistic regression** and other classification models to evaluate the lending data.

The analysis is implemented in **Jupyter Notebook** and uses **pandas**, **scikit-learn**, and **imbalanced-learn** for data preprocessing, model training, and evaluation.

---

## Data Files

| File Name                   | Description                                      |
|-----------------------------|--------------------------------------------------|
| `lending_data.csv`          | Dataset containing historical lending data, including loan amounts, interest rates, and risk levels. |
| `credit_risk_classification.ipynb` | Jupyter Notebook for training and evaluating machine learning models. |

---

## Features

1. **Data Preprocessing**:
   - Loads and cleans lending data.
   - Encodes categorical variables and scales numerical features.

2. **Model Training**:
   - Applies machine learning models:
     - Logistic Regression
     - Random Forest Classifier
     - Other classification models as needed.

3. **Model Evaluation**:
   - Evaluates performance using accuracy, precision, recall, and F1-score.
   - Handles class imbalances using resampling techniques (SMOTE).

4. **Comparison of Results**:
   - Compares different models and techniques to determine the best-performing classifier.

---

## Installation

1. **Prerequisites**:
   - Python 3.x
   - Jupyter Notebook

2. **Setup**:
   - Clone this repository or download the project files.
     
   - Install dependencies (if needed):
     ```bash
     pip install -r requirements.txt
     ```
---

## Results

### Key Observations:
* The logistic regression model provides baseline performance for credit risk classification.
* Advanced models, such as Random Forest and SMOTE techniques, improve classification accuracy, especially in imbalanced datasets.

Model Evaluation:
* Accuracy, Precision, Recall, and F1-Score are used to compare model performance.

	•	Logistic Regression Model:
	•	Accuracy: 99%
	•	Class 0 (Healthy Loan):
	•	Precision: 1.00
	•	Recall: 0.99
	•	F1-score: 1.00
	•	Class 1 (High-Risk Loan):
	•	Precision: 0.86
	•	Recall: 0.94
	•	F1-score: 0.90

---

## Overview of the Analysis

The purpose of this analysis is to classify loan applications as either “healthy” (low risk) or “high risk” using a logistic regression model. The dataset includes financial information about borrowers, such as loan size, interest rate, and borrower income. The objective is to predict the likelihood of a loan being high-risk based on these factors.

Key aspects of the dataset:
	•	Target Variable: loan_status (0 = healthy loan, 1 = high-risk loan)
	•	Data Summary: The dataset is imbalanced, with most loans categorized as “healthy.”

Machine learning process stages:
	1.	Data Loading and Preprocessing: Loaded and cleaned data, separated labels and features.
	2.	Data Splitting: Used train_test_split to divide the dataset into training and testing sets.
	3.	Model Training: Trained a LogisticRegression model on the training data.
	4.	Model Evaluation: Used a confusion matrix and classification report to assess accuracy, precision, and recall.
---

## Summary

The logistic regression model performs exceptionally well, with an overall accuracy of 99%. It predicts healthy loans with near-perfect precision and recall, while also achieving high recall (0.94) for high-risk loans. Given the class imbalance, the model still accurately identifies high-risk loans, which may be crucial for reducing financial risk.

The logistic regression model is recommended due to its strong performance in identifying both healthy and high-risk loans. In cases where accurate identification of high-risk loans is prioritized, the model’s high recall for 1 makes it suitable for credit risk classification.

---

## Author

**Kendall Burkett**  
https://github.com/KendallBurkett?tab=repositories
 
kbz1987@icloud.com
