# Module 12 Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this analysis is to improve our banks ability to predict loan defaulting.

* Explain what financial information the data was on, and what you needed to predict.

* The data that was provided included loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, and total debt. Using these variable we created a ML model to aid in the prediction of future high risk loans. 

* In the provided data set there was an imbalance of high risk loans(2500) and secure loans(75036).

* All the data was seperated into test and train to allow me to test me model on different data to ensure that the model could properly place future loan candidates. Then, the train data was fit to the model and prediction were extracted from the trained models. 

* The model used for categorizing individual into high risk loan or not was the LogisticRegression model which uses Logistic Regression to place data point into one category or an other. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * Accuracy: The Model was accurate 95% of the time, determining the correct category for the individual in the dataset.
  * Precision: Out of all the loans the model predicted would default 85% of them did.
    * Recall: Out of all the loans that did default, the model predicted this outcome 91% of the time


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Accuracy: The Model was accurate 99% of the time, determining the correct category for the individual in the dataset. This is an improvement over the first model.
  * Precision: Out of all the loans the model predicted would default 84% of them did.(slightly worse than the previous model.)
  * Recall: Out of all the loans that did default, the model predicted this outcome 99% of the time.(An improvement from the previous model.)

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The second model preformed better in almost all cases and in the slight dip in preformance in precision is acceptable as Recall is more important to the bank as giving risky loans has higher associated risk.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Yes the preformance of the model could depend on the type of problem we are solving, however there does seem to be a general improvement from the first model to the second. 

If you do not recommend any of the models, please justify your reasoning.

Yes, I recommend the second model. The second model had a high accuracy and recall allowing banks to avoid risky loan and having clients default leading to extra risk for the bank. Using this model the bank would be able to improve their ability to mitigate risk. 
Assuming that the value counts from the dataset represent the banks ability to determine risk without the model they currently give out risky loans 3% of the time. By reducing this number by possibily 2% gains for the corpertation could be substantial. 