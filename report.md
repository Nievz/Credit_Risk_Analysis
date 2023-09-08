# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

Credit risk poses a classification problem that’s inherently imbalanced. The reason is that healthy loans easily outnumber risky loans. The purpose of this analysis is to develop various techniques to train and evaluate models with imbalanced classes. We use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

To conduct the analysisi we:

    Split the Data into Training and Testing Sets
    
        Examine the balance of the labels variable (y) by using the value_counts function.

    Create a Logistic Regression Model with the Original Data

    Predict a Logistic Regression Model with Resampled Training Data

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
 The logistic regression model used to analyze the data predicts a higher probability for healthy loans than for high risk loans. The prediction on the healthy loan is significant, with better scores in precision, recall, and f1.
 
 precision    recall  f1-score   support

Class Purple       1.00      0.99      1.00     18765
Class Yellow       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
 The logistic regression model that was applied to the data from the oversampling did, in fact, predict a better probability to the high risk loan than the model that was applied to the original data. An improvement could be seen in both the prediction's recall and its F1 score, with recall going from 0.91 to 0.99 and frequency going from 0.88 to 0.91. On the other hand, there was not a significant change in the healthy loan ratings.
  
   precision    recall  f1-score   support

Class Purple       1.00      0.99      1.00     18765
Class Yellow       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

After conducting our analysis, we recommend using a logistic regression with random over sampling because it predicts a higher probability of the high risk loan than the model used on the original data. The prediction's recall and F1 score both improved, with recall increasing from 0.91 to 0.99 and F1 increasing from 0.88 to 0.91. Healthy loan ratings, on the other hand, did not change significantly.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

We believe that it is preferable to have a model that predicts a higher probability on the high risk loans because the impact on the company would be greater if those loans were not identified properly. 

If you do not recommend any of the models, please justify your reasoning.
