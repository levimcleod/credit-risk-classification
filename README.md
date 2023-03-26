
## Overview of the Analysis

The purpose of the analysis is to produce a model that can predict whether a loan applicant correlates to high-risk or low-risk borrowing behavior. 

The data used in the model was harvested from a peer-to-peer lending service containing historical lending data. 

The variable we targeted for our predictions was the loan status, be it "Healthy" or "High-risk".

Steps:

- Separate data into labels and features
- Split data into training and testing subsets
- Instantiate, fit, and predict using a LogisticRegression module
- Evaluate model's performance with balanced accuracy, confusion matrix, and classification report
- Repeat above steps using resampled data from RandomOversampler

## Results

* LR_Model 1:
  * The model predicts healthy and high-risk loans with almost perfect (99%) weighted accuracy, precision, and recall.

* LR_Model 2:
  * The LR model fit with oversampled data predicted the healthy and high-risk loans with a greater macro average recall (from 0.95 to 0.99).This means that this model is better at minimizing false negatives. The weighted averages are the same for both models.

## Summary

The logistic regression model we created performs with high accuracy, precision, and recall. When resampled, our second model performed with an even higher recall (From 0.95 to 0.99). 

The choice of model is dependent on the use case, but using our LR_Model 2 will minimize false negatives. This makes the second model a more appropriate model for use cases such as the medical field. However, both of the models make predictions with 99% weighted accuracy.

