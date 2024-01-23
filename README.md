# 20-credit-risk-classification

# Coding file 


# Report

## Overview of the Analysis

* The purpose of the analysis is to tell us how accuary the model can predict for classification between healthy loan and high-risk loan.
* The values we need to input are loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total debt. After taking those value, the model can help us predict the loan is belong to healthy loan or high risk loan.
* After using value_counts, we know that there are 75036 healthy loan and 2500 high risk loan in the dataset.
* The first machine learning process I had were split the data into training and testing datasets using train_test_split. 
* I used the LogisticRegression method to create a lr_model, train the lr_model with the training data, do a prediction using the lr_model, use balanced accuracy score, confusion matrix, classification report to see how well the model is.
* Also, I used RandomOverSampler to get a oversize sample dataset and use the LogisticRegression method as above.

## Results

* The Logistic Regression Model(with the Original Data):
  * The Model with original data has accuracy as 0.99, precision of healthy loan as 1.00, precision og high-risk loan as 0.85, recall of healthy loan as 0.99, and recall of high-risk loan as 0.91.



* The Logistic Regression Model(with the oversampled data):
  * The Model with oversampled data has accuracy as 0.99, precision of healthy loan as 1.00, precision og high-risk loan as 0.84, recall of healthy loan as   0.99, and recall of high-risk loan as 0.99.

## Summary
* Both models have the accuracy as 0.99, therefore, both models are good models for using to predict the loan belong to healthy loan or high-risk loan.
* Both models are well for predicting the healthy loan, since both models have the same high accuarcy, precision, and recall.
* For predicting the high risk loan, the model with oversample is better since it has the precision 0.84 which is lower than the model with original data by 0.01, but it has the recall as 0.99 which is higher than the model with original data by 0.08.
