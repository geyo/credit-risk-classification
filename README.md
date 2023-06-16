# Credit Risk Classification

By Grace Yoo

**Programming Languages & Libraries Used:** Python, pathlib, pandas, sklearn

**Concepts:** Supervised Learning, Classification, Logistic Regression

## Purpose

The purpose of this project is to train and evaluate a model based on loan risk that can identify the creditworthiness of borrowers. 

## Data Background and What To Predict

The dataset has historical lending activity from a p2p lending services company. The purpose of this model is to predict the creditworthiness of borrowers. 

## Variables to Predict

The variable we are trying to predict is the loan status. This is a binary variable--either 0 (healthy loan) or 1 (high risk of defaulting.)

## Machine Learning Process

The steps of the machine learning process were as follows:
Step 1: Preprocess the data
The data was split into training and testing sets. 
Step 2: Train the model using training dataset. 
Step 3: Validate the model by making a prediction as to what the loan status would be and comparing it to the actual loan value. Generate an accuracy score, confusion matrix and classification report for the model. 

This was done first with a logistic regression model with the original data, and redone using resampled training data that were modified with the 'random over sampler" model. 

The logistic regression model was used to fit the data. For the second try, the data was altered using the 'randomoversampler' model. 

## Results

The balanced accuracy scores, precision and recall scores of all machine learning models were as follows: 

* Machine Learning Model 1 (Logistic Regression):
  * Accuracy score: .99
  * Precision for High-Risk Loan: .87
  * Precision for Healthy Loan: 1.00
  * Recall for High-Risk Loan: .89
  * Recall for Healthy Loan: 1.00
 
* Machine Learning Model 2 (Logistic Regression with Resampled Training Data):
  * Accuracy score: 1.00
  * Precision for High-Risk Loan: .87
  * Precision for Healthy Loan: 1.00
  * Recall for High-Risk Loan: 1.00
  * Recall for Healthy Loan: 1.00  


### Summary

The second learning model seems to perform the best as the accuracy score is higher. 

Performance changes based on the problem to solve. If we are trying to predict high-risk loans (1), the second model might be better, as recall is 1 as opposed to .89. If we are trying to predict healthy loans, either model will work. 
