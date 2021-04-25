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
As shown in the result session, all 6 machine learning models have 1.00 precision for low-risk, meaning that they are reliable on predicting low-risk cases. But most of them are bad at precisely predicting high-risk cases. All resampling models got 0.01 precision score for high-risk. Two ensemble algorithms got 0.03 and 0.09 precision scores. All models except for Easy Ensemble AdaBoost Classifier got recall lower than 0.75 for predicting high-risk cases, meaning that they can only find lower than 75% of the high-risk cases out of all the high-risk cases. The recall for Easy Ensemble AdaBoost Classifier is 0.92, so it can find 92% of the high-risk cases, it also got the highest recall for predicting low-risk cases. 

I recommend Easy Ensemble AdaBoost Classifier since it can successfully find most of the high-risk and low-risk cases, although the precision for high-risk is only 0.09, but future verification after the screening can be used to furthur determine whether the case is in high-risk.


