# Module 20 README

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

## Results

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

## Summary

The logistic regression model performs exceptionally well, with an overall accuracy of 99%. It predicts healthy loans with near-perfect precision and recall, while also achieving high recall (0.94) for high-risk loans. Given the class imbalance, the model still accurately identifies high-risk loans, which may be crucial for reducing financial risk.

The logistic regression model is recommended due to its strong performance in identifying both healthy and high-risk loans. In cases where accurate identification of high-risk loans is prioritized, the model’s high recall for 1 makes it suitable for credit risk classification.
