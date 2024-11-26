# Module 12 Report Template

## Overview of the Analysis

The purpose of the analysis is to devise a supervised machine learning model that will predict if a loan is healthy (class 0) or high-risk (class 1). The employment of a logistic regression as a binary classification method for our model was used in this analysis. The investigation focused on financial data, particularly examining factors such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The goal was to determine the loan status, categorizing it as either a healthy loan (0) or a high-risk loan (1). The dataset utilized comprises a CSV file containing 77,500 entries. 
The dataset was divided into labels and features, designating loan status (either healthy or high-risk) as the label and the other seven columns as features. Subsequently, the data was partitioned into training and testing datasets. A Logistic Regression model from sklearn was utilized. Logistic Regression was selected as a binary classifier since we are categorizing loans as either healthy or high-risk, with only these two alternatives. The model was then trained using the training data. Predictions were generated based on the test data. The effectiveness of the model was assessed through accuracy, precision, and recall scores.

## Results

The model achieves an overall accuracy of 0.99, meaning it successfully classifies 99% of the cases.

Its precision to determine:

Healthy Loan (class 0): 1.00  
High-Risk Loan (class 1): 0.85  

Its recall:

Healthy Loan (class 0): 0.99  
High-Risk Loan (class 1): 0.91  

## Summary

The logistic regression model did a good job at identifying healthy loans (class 0), achieving a precision of 1.00 and a recall of 0.99. In contrast, when it comes to risky loans (class 1), the model had a precision of 0.85 and a recall of 0.91. The decreased precision and recall for predicting risky loans (class 1) could be due to the imbalanced nature of the dataset, as there are only 619 support test data points for class 1, which is significantly lower than 18765 for class 0. There is room for improvemnet in the prediction of high-risk loans. The model has limited exposure to high-risk loans relative to the number of healthy loans in the dataset. In regards to loan classification, it is more critical to prevent high-risk loans than to issue loans, as the financial loss from a single defaulted loan can exceed the interest gained from a loan. The total accuracy of the model stands at 99%.
