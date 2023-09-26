# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

- The aim of this assessment is to assess the effectiveness of two logistic regression machine learning models in forecasting the credit risk linked to loans. This evaluation was carried out using financial data that includes information on loan amounts, interest rates, borrowers' incomes, debt-to-income ratios, the number of accounts, derogatory marks, and total debt. The primary goal was to make predictions about the status of the loans, categorizing them as either low-risk ('0') or high-risk ('1').

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
- The accuracy is at 0.95
- The precision is at 1 at healtly loan(0) and 0.86 at high-risk loan (1).
- The recall, it is at 0.99 at healtly loan(0) and 0.91 at high-risk loan (1). 


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
- The accuracy is at 0.99
- The precision is at 0.99 at healtly loan (0) and 0.99 at high-risk loan(1)
- The recall, it is at 0.99 at healtly loan (0) and 0.99 at high-risk loan (1).

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

After reviewing the outcomes of our modeling efforts, it became evident to me that the secondary logistic regression model, which was trained using resampled data, outperformed the initial model trained on the original dataset. This was especially noticeable in its ability to predict high-risk loans ('1'). The second model exhibited significantly higher precision, recall, and F1 scores when it came to identifying high-risk loans. This particular aspect of performance is of utmost importance to assist the lending company in mitigating bad loans and minimizing financial losses.

Given these findings, I strongly recommend the adoption of the second model, which utilizes logistic regression and is trained with resampled data, for our credit risk analysis. The improved accuracy of this model compared to the first one is quite evident. The results indicate its capability to more effectively differentiate between healthy loan applications and high-risk ones, thereby helping us avoid granting loans that could result in greater future losses.