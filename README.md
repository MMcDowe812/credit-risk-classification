# credit-risk-classification
# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
    The purpose of the Logistics Regression Model is to predict whether a borrow will be taking out a healthy loan or a high risk loan by placing a predicting indicator, in this case a 0 for healthy and a 1 for High Risk, next to the load information
* Explain what financial information the data was on, and what you needed to predict.
    Data was in a CSV file and multiple libraries such as Numpy, Pandas, Pathlib (to read the CSV file), and sklearn to train the model.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
    Model is trained to predict if the loan will be healthy or risky
* Describe the stages of the machine learning process you went through as part of this analysis.
    First stage is to separate the data that we are trying to predict from the file.  In this case we are predicting healthy and high risk loans.  The CSV file contains other variables to train the model such as loan size, borrower income, debt to income ratio, etc.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms). 
    In this assignment Logistic Regression was the only model used due to the multiple numeric values.  This model predicted with a high accuracy.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    -Description of Model 1 Accuracy, Precision, and Recall scores.
    * The accuracy was calculated at 99% per the classification report.  This measured the test data up against the data that was split from the model and not seen by the machine.  
    * The precision in the classfication report had a 100% for the healthy loans (0) and an 85% for the high-risk loans (1).  This indicates that if the model predicts a 0 you can trust it fully.  If it produces a 1, then there is a margin of error that it could still be a good loan but the information the model produces, can be trusted by the user.
    * Recall is a tool to minimize the false negatives.  The healthy loan had 99% compared to 91% for the high risk.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best? 
    Only used Logistics and it had a 100% on healthy loans with an overall of 99% accuracy.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )  
    In this model, it's more important to predict the 0s.  If the model falsely predicts a high risk, this protects the user vs the other predictor.

If you do not recommend any of the models, please justify your reasoning.