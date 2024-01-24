# credit-risk-classification
Module 20 - Supervised Machine Learning

## Overview of the Analysis

The purpose of this analysis was to assess the credit value of loan borrowers, to determine if their loan status (approved, denied) by count (binary results) via the machine learning model using logistic regression from sklearn.metrics. The data that was used as training data included the following columns:

```
"loan_size","interest_rate","borrower_income","debt_to_income",
"num_of_accounts","derogatory_marks","total_debt"
```
which produced the output: "loan_status". After the model was trained, a balanced accuracy test was ran to see the credibility of the results, followed by a confusion matrix which reported how many true positives, false positives, true negatives, false negatives were made by the model. A classification report was then ran for quality check, to get a better overview of the confusion matrix results.

After this process was completed, another logistic regression model was ran after utlizing RandomOverSampler, and all the steps in the first half were repeated. The purpose of this step was to see how well the loogistic regression model predicts with oversampled data. 

## Results

The balanced accuracy scores and the precision and recall scores of both machine learning models.

Machine Learning Model 1:
  * Accuracy: 0.94
    - This accuracy report is a good indicator of the model being credible 
  * Precision: 1.00 (for value of 0) 0.87 (for value of 1)
    - These values show how the model responded for values of 1 and 0, where it
      correctly producing results for 0, 100% of the time, meanwhile 87% of the
      time for 1. 
  * Recall scores: 1.00 (for value 0) 0.89 (for value of 1)



* Machine Learning Model 2 (oversampled data):
  * Accuracy: 0.99
  * Precision: 0.99 (for both binary values)
  * Recall scores: 0.99 (for both binary values)`

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
