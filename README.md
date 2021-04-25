# An Analysis on the performance of different machine learning model on predicting credit risk

## Overview of the analysis
The purpose of this analysis is to evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

### Oversampling
- The accuracy score for naive random oversampling method is 0.6627967286906427, the classification report is shown below. The precision and recall for predicting high-risk are 0.01 and 0.69. The precision and recall for predicting low-risk are 1.00 and 0.61.

![NRO](/Images/NRO.png)

- The accuracy score for SMOTE method is 0.6622771929905806, the classification report is shown below. The precision and recall for predicting high-risk are 0.01 and 0.63. The precision and recall for predicting low-risk are 1.00 and 0.69.

![SMOTE](/Images/SMOTE.png)

### Undersampling
- The accuracy score for undersampling method is 0.5442661782548694, the classification report is shown below. The precision and recall for predicting high-risk are 0.01 and 0.69. The precision and recall for predicting low-risk are 1.00 and 0.40.

![Undersampling](/Images/Undersampling.png)

### Combination
- The accuracy score for combination sampling method is 0.6447993752836463, the classification report is shown below. The precision and recall for predicting high-risk are 0.01 and 0.72. The precision and recall for predicting low-risk are 1.00 and 0.57.

![Combination](/Images/Combination.png)

### Ensemble algorithms
- The accuracy score for Balanced Random Forest Classifier is 0.7672346923654012, the classification report is shown below. The precision and recall for predicting high-risk are 0.03 and 0.67. The precision and recall for predicting low-risk are 1.00 and 0.86.

![BRFC](/Images/BRFC.png)

- The accuracy score for Easy Ensemble AdaBoost Classifier is 0.932975553168039, the classification report is shown below. The precision and recall for predicting high-risk are 0.09 and 0.92. The precision and recall for predicting low-risk are 1.00 and 0.95.

![AdaBoost](/Images/AdaBoost.png)

## Summary
