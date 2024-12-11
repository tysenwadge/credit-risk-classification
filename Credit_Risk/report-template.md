# Credit Risk Analysis Report

## Overview of the Analysis

Lending companies lend assets to borrowers expecting that the borrower will repay what was lended. Credit Risk is the result of a borrower not returning an asset or paying back a loan, resulting in the lender losing money. In this challenge, I will use Machine Learning to analyze a dataset of historical lending activity from a peer-to-peer lending services company to build a model that will identify the Credit Risk of borrowers.

The purpose of this analysis is to create a supervised machine learning model that will predict if a loan is healthy '0' or high-risk '1'. I will use logistic regression to accomplish this. The data being analyzed focuses on loan size, interest rate, borrower's income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. 

* Using Machine Learning, I will try to predict which loans are healthy (low-risk) or non-healthy (high-risk) based on the loan status provided. First I need to split the data into labels and features, loan status being the label and the remaining columns as the features. The data then gets split into training and test data sets. Next, a logistic regression model gets initialized since we are classifying loans as either healthy or high-risk. The model was then fit with the training data and predictions were made. Finally, I evaluated the models performance using accuracy, precision, and recall scores.  
## Results

Description of metrics used to evaluate the models performance:

* Accuracy, Precision, and Recall:
    * Accuracy: The overall accuracy of the model is 0.99, meaning that it correctly classify's or predicts 99% of instances.
    * Precision: Healthy Loan ('0') ~ 1.00, High-Risk Loan ('1') ~ 0.84
    * Recall: Healthy Loan ('0') ~ 0.99, High-Risk Loan ('1') ~ 0.94

## Summary

Overall, the model is performing very well in predicting healthy loans, as seen by the precision score of 1.00, and recall score of 0.99. The high-risk loans, however, resulted in a precision score of 0.84, and recall of 0.94.

With that being said, the support test data for high-risk loans is only 619, compared to the support test data for healthy loans of 18765. The model could be improved by training it with more high-risk loans. 

When it comes to classifying loans, it is more important to determine and prevent high-risk scenarios as defaulting can result in a larger loss compared to potential interest to be earned. I would recommend the logisitic regression model be used as it is performing with an overall accuracy of 99%.