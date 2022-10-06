# Credit_Risk_Analysis

## Overview
The goal in this project was to use Machine Learning to identify the risk for each application that applies for a credit card. I used Supervised Machine Learning to help predict credit risk. A very important tool for banks and any establishment that relies on credit. However, I used multiple algorithms to resample the data. Often times, data can create biases towards a majority or a minority set in the data. To avoid that, I have used the following algorithms:

1. RandomOverSampler
2. SMOTE
3. ClusterCentroids
4. SMOTEENN
5. BalancedRandomForestClassifier
6. EasyEnsembleClassifier

in that order. So let's see which one we can depend on the most.

## Results
Without further ado, I present the data to you.

### RandomOverSampler
![NaiveOver](https://github.com/Aceofhearts1/Credit_Risk_Analysis/blob/main/Images/OverSampling.png)

- Balanced Accuracy: 64.71%
- High Risk - precision rate: 1% recall: 62% F1: 2%
- Low Risk - precision rate:  100% recall: 67% F1: 80%

### SMOTE
![Smote](https://github.com/Aceofhearts1/Credit_Risk_Analysis/blob/main/Images/SMOTE.png)

- Balanced Accuracy: 62.51%
- High Risk - precision rate: 1% recall: 62% F1: 2%
- Low Risk - precision rate: 100% recall: 63% F1: 77%

### ClusterCentroids
![UnderSample](https://github.com/Aceofhearts1/Credit_Risk_Analysis/blob/main/Images/UnderSampling.png)

- Balanced Accuracy:
- High Risk - precision rate: 1% recall: 57% F1: 1%
- Low Risk - precision rate: 100% recall: 46% F1: 63%

### SMOTEENN
![Smoteenn](https://github.com/Aceofhearts1/Credit_Risk_Analysis/blob/main/Images/Combination.png)

- Balanced Accuracy: 51.88%
- High Risk - precision rate: 1% recall: 70% F1: 2%
- Low Risk - precision rate:  100% recall: 58% F1: 73%

### BalancedRandomForestClassifier
![BRF](https://github.com/Aceofhearts1/Credit_Risk_Analysis/blob/main/Images/BalancedRandomF.png)

- Balanced Accuracy: 78.78%
- High Risk - precision rate: 4% recall: 67% F1: 7%
- Low Risk - precision rate: 100% recall: 91% F1: 95%

### EasyEnsembleClassifier
![EE](https://github.com/Aceofhearts1/Credit_Risk_Analysis/blob/main/Images/EasyEnsemble.png)

- Balanced Accuracy: 92.54%
- High Risk - precision rate: 7% recall: 91% F1: 14%
- Low Risk - precision rate: 100% recall: 94% F1: 97%

## Summary
With all of the data and models captured, we can see with algorithm best works out for us. The model to use for our machine learning credit risk is the Easy Ensemble Classifier. It had the best balance of all of the models. The highest precision rate for high risk, the high recall/ sensitivity rate, and highest F1 score. We've have seen that we can teach a machine learning model to help identify who to accept and who to decline with credit applications.