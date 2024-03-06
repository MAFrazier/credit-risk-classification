# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

#### Purpose of analysis is to develop machine learning models that predicts loan status based on financial information provided in the dataset. The dataset included the following information: loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status (0 for healthy loan, 1 for high-risk loan).

#### The data was then split into  split (X) and labels (y); where X contains all features from original dataset except the loan status column, and y contains only the loan status column.

#### Then two logistic regression models was trained. The first model was trained on the original data, while the second model was trained on resampled data obtained using RandomOverSampler to address the class imbalance issue that was observed, where majority were healthly loans compared to high-risk loans

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

#### Machine Learning Model 1:

        * Balanced accuracy score: 0.95
        * Precision and Recall for label 0 (healthy loan):
        * Precision: 1.00
        * Recall: 0.99
        * Precision and Recall for label 1 (high-risk loan):
        * Precision: 0.85
        * Recall: 0.91

#### Machine Learning Model 2:

        * Balanced accuracy score: 0.99
        * Precision and Recall for label 0 (healthy loan):
        * Precision: 0.99
        * Recall: 0.99
        * Precision and Recall for label 1 (high-risk loan):
        * Precision: 0.99
        * Recall: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


#### Both machine learning models performed well in predicting loan status. However, the second model trained on resampled data achieved slightly higher accuracy, precision, and recall scores compared to the model trained on the original data first Model . So, addressing the class imbalance issue through resampling improved the model's performance.

#### Since it is very important to accurately predict high-risk loans, then resampled Model would be preferred due to its higher precision and recall for this label. 

#### The second model would be recommend based on the higher performance and its ability to effectively predict both healthy and high-risk loans.





