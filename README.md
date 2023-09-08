# Credit_Risk_Analysis

<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name=" Rental-Market-Data-San-Fran"></a>
<img src="https://github.com/Nievz/Credit_Risk_Analysis/blob/main/Images/banner.jpg" alt="Logo" width="1000" height="450">

<!-- ABOUT THE PROJECT -->
## Overview of the Analysis

  <p align="center"> 
    Credit risk poses a classification problem that’s inherently imbalanced. The reason is that healthy loans easily outnumber risky loans. The purpose of this analysis is to develop various techniques to train and evaluate models with imbalanced classes. We use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
  </p>

  <p align="center" style="display: flex;" >
<img src="https://github.com/Nievz/Credit_Risk_Analysis/blob/main/Images/logo.png" alt="Logo" width="50" height="50">  
<img src="https://img.shields.io/npm/l/express" />
<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/tyleradammartinez/SIG-Dashboard-Application" />
    <img src="https://github.com/Nievz/Credit_Risk_Analysis/blob/main/Images/logo.png" alt="Logo" width="50" height="50"> 
</p>


## To conduct the analysis we:
* Split the Data into Training and Testing Sets.
    * Examine the balance of the labels variable (y) by using the value_counts function.
* Create a Logistic Regression Model with the Original Data
* Predict a Logistic Regression Model with Resampled Training Data
    
## Results

  We describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
 The logistic regression model used to analyze the data predicts a higher probability for healthy loans than for high risk loans. The prediction on the healthy loan is significant, with better scores in precision, recall, and f1.
 

<img src="https://github.com/Nievz/Credit_Risk_Analysis/blob/main/Images/table1.png" alt="Logo" width="900" height="300">


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  
 The logistic regression model that was applied to the data from the oversampling did, in fact, predict a better probability to the high risk loan than the model that was applied to the original data. An improvement could be seen in both the prediction's recall and its F1 score, with recall going from 0.91 to 0.99 and frequency going from 0.88 to 0.91. On the other hand, there was not a significant change in the healthy loan ratings. <br>
  
<img src="https://github.com/Nievz/Credit_Risk_Analysis/blob/main/Images/table2.png" alt="Logo" width="900" height="300">

## Summary

We summarize the results of the machine learning models, and include a recommendation on the model to use:
* Which one seems to perform best? How do we know it performs best?

After conducting our analysis, we recommend using a logistic regression with random over sampling because it predicts a higher probability of the high risk loan than the model used on the original data. The prediction's recall and F1 score both improved, with recall increasing from 0.91 to 0.99 and F1 increasing from 0.88 to 0.91. Healthy loan ratings, on the other hand, did not change significantly.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

We believe that it is preferable to have a model that predicts a higher probability on the high risk loans because the impact on the company would be greater if those loans were not identified properly. 


<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [https://realpython.com/logistic-regression-python/]()
* [https://towardsdatascience.com/building-a-logistic-regression-in-python-step-by-step-becd4d56c9c8]()
* [https://aws.amazon.com/what-is/logistic-regression/]()
