# credit-risk-classification
module-20-challenge 

Used intructor videos and supervised learning notebooks to complete this assignment

# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
    * The goal of this analysis is to determine if the Logistic Regression model can be accurate to predict healthy loans versus high risk loans. This involved comparing original data versus resampled data to increase the size of the minority class in order to balance the data.
* Explain what financial information the data was on, and what you needed to predict.
    * The data was based on loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, and total_debt, and loan status. The prediction was the loan status.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
    * The value counts for the original data were 75,036 for healthy loans and 2500 for high-risk loans.
    * The value counts for the oversampled data were 56,271 for healthy loans and 56,271 for high-risk loans.
* Describe the stages of the machine learning process you went through as part of this analysis.
    1. We first prepared the data by moving it into pandas.
    2. We separated the data into columns, where X and y determined the output.
    3. We then train_test_split the data.
    4. We then picked machine learning models using LogisticRegression for classification.
    5. We then fit the model with training data.
    6. We then used the model to make predictions with the test data.
    7. We then looked at the performance of our models, looking at the balanced accuracy score, confusion matrix, and classification report.
    We then used the model to make predictions
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
    * We used the following methods:
        * SKLearn Logistic Regression
        * train_test_split function
        * balanced_ccuracy_score
        * confusion_matrix
        * classification_report

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
* Description of Model 1
* Accuracy: 0.99
* Class 0 - Healthy Loans
    * Precision: 1.00
    * Recall: 0.99
* Class 1 - High-Risk Loans
    * Precision: 0.84
    * Recall: 0.94



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
* Description of Model 2
* Accuracy: 0.99
* Class 0 - Healthy Loans
    * Precision: 1.00
    * Recall: 0.99
* Class 1 - High-Risk Loans
    * Precision: 0.84
    * Recall: 0.99
    
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
    * For class 0, the LogisticRegression model performed with virtually 100% accuracy. For class 1 with the original data, we see a precision of 84% and a recall of 94%. This shows a strong indicator that the machine learning model was fairly accurate and performed well. 
    
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
    * It is more important to the predict the 1's as the high-risk loans need to be identified. Therefore the performance is shown as better since the LogisticRegression model shows a high recall value, meaning it is more likely to show a false positive than a false negative. This in turn will reveal moree 1's.

If you do not recommend any of the models, please justify your reasoning.
    * Overall the LogisticRegression models do a great job of predicting the healthy and high risk loans. I would not recommend this model immediately. The LogisticRegression model may look promising, as it performed well for this dataset, but it would need to be applied to additional datasets to confirm its accuracy and usability.
