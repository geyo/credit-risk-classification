# Module 12 Report Template

## Overview of the Analysis

* Explain the purpose of the analysis.
The purpose of this analysis is to train and evaluate a model based on loan risk. 

* Explain what financial information the data was on, and what you needed to predict.
The dataset has historical lending activity from a p2p lending services company. The purpose of this model is to predict the creditworthiness of borrowers. 

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The variable we are trying to predict is the loan status. This is a binary variable--either 0 (healthy loan) or 1 (high risk of defaulting.)

* Describe the stages of the machine learning process you went through as part of this analysis.
The steps of the machine learning process were as follows:
Step 1: Preprocess the data
The data was split into training and testing sets. 
Step 2: Train the model using training dataset. 
Step 3: Validate the model by making a prediction as to what the loan status would be and comparing it to the actual loan value. Generate an accuracy score, confusion matrix and classification report for the model. 

This was done first with a logistic regression model with the original data, and redone using resampled training data that were modified with the 'random over sampler" model. 

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
THe logistic regression model was used to fit the data. For the second try, the data was altered using the 'randomoversampler' model. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * Accuracy score: .99
  * Precision for High-Risk Loan: .87
  * Precision for Healthy Loan: 1.00
  * Recall for High-Risk Loan: .89
  * Recall for Healthy Loan: 1.00
 
* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Accuracy score: 1.00
  * Precision for High-Risk Loan: .87
  * Precision for Healthy Loan: 1.00
  * Recall for High-Risk Loan: 1.00
  * Recall for Healthy Loan: 1.00  


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The second learning model seems to perform the best as the accuracy score is higher. 

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Performance changes based on the problem to solve. If we are trying to predict high-risk loans (1), the second model might be better, as recall is 1 as opposed to .89. If wer are tryign to predict healthy loans, either model will work. 

