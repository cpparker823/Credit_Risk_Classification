Overview of the Analysis

The purpose of this analysis is to build a predictive model to determine whether a loan needs to be classified as "healthy" or "high risk." 
I used supervised machine learning skills to analyze creditworthiness variables (such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt) for each instance.
I started by splitting a raw dataset into training and testing sets. Then I created a logistic regression model to make predictions. I followed up the predictive model with a confusion matrix and classification report to analyze its performance.

Results

Classification Report
              precision    recall  f1-score   support

     Healthy       1.00      0.99      1.00     18765
   High-Risk       0.85      0.91      0.88       619
    accuracy                           0.99     19384

    -The precision score for predicting healthy loans was 100%
    -The precision score for predicting high risk loans was 85%
    -The recall score for healthy loans was 99%
    -The recall score for high risk loans was 91%
    -The overall accuracy for the model in predicting both healthy and high risk loans was 99%

Summary

While the model performs at a high success rate, it is important to note the difference between healthy loan predicitons (100%) and high risk (85%). The model seems to favor predicting borderline loans as healthy when perhaps it should err on the side of caution. Missing 15% of high risk loans could result in unforseen default liabilities to the lender. I would like to see this model perform more conservatively before recommending it be used or relied upon by the company. 
