# Credit Risk Analysis

## Overview

The purpose of this project is to use machine learning to help evaluate credit card risk using a file of loan applications and their statuses and evaluate which model works best on such an imbalanced dataset. The data needs to be balanced to achieve reliable results and will use oversampling with the RandomOverSampler and SMOTE algorithms, undersampling with the ClusterCentroids algorithm, and a combo approach of over and undersampling with the SMOTEENN algorithm. Two bias reduction algorithims are then compared, BalancedRandomForestClassifier and EasyEnsemble AdaBoost algorithms. The balanced accuracy scores and precision and recall scores will be used to compare the six algorithms. 

## Resources

- Data: LoanStats_2019Q1.csv
- Software: Jupyter Notebook 6.4.8; Python 3.7.13; Imbalanced-Learn Library 0.9.0; SciKit-Learn Library 1.0.2

## Results

### Naive RandomOverSampler Model

![randomoversampling](https://github.com/mein0819/Credit_Risk_Analysis/blob/main/readMeImages/naiveOverSampling.png)

- Balanced Accuracy Score: 63%
- Precision High-Risk: 1%
- Precision Low-Risk: 100%
- Recall High-Risk: 57%
- Recall Low-Risk: 68%

### SMOTE Oversampling

![smote](https://github.com/mein0819/Credit_Risk_Analysis/blob/main/readMeImages/smoteOversampling.png)

- Balanced Accuracy Score: 63%
- Precision High-Risk: 1%
- Precision Low-Risk: 100%
- Recall High-Risk: 57%
- Recall Low-Risk: 68%

### ClusterCentroids Resampling

![cluster](https://github.com/mein0819/Credit_Risk_Analysis/blob/main/readMeImages/clusterCentroids.png)

- Balanced Accuracy Score: 53%
- Precision High-Risk: 1%
- Precision Low-Risk: 100%
- Recall High-Risk: 61%
- Recall Low-Risk: 45%

### SMOTEENN Over- and Undersampling

![smoteenn](https://github.com/mein0819/Credit_Risk_Analysis/blob/main/readMeImages/smoteenn.png)

- Balanced Accuracy Score: 65%
- Precision High-Risk: 1%
- Precision Low-Risk: 100%
- Recall High-Risk: 70%
- Recall Low-Risk: 61%

### Balanced Random Forest Classifier

![brfc](https://github.com/mein0819/Credit_Risk_Analysis/blob/main/readMeImages/balancedRFC.png)

- Balanced Accuracy Score: 77%
- Precision High-Risk: 3%
- Precision Low-Risk: 100%
- Recall High-Risk: 66%
- Recall Low-Risk: 88%

### Easy Ensemble AdaBoost Classifier

![adaboost](https://github.com/mein0819/Credit_Risk_Analysis/blob/main/readMeImages/adaBoost.png)

- Balanced Accuracy Score: 92%
- Precision High-Risk: 9%
- Precision Low-Risk: 100%
- Recall High-Risk: 89%
- Recall Low-Risk: 94%

## Summary

After reviewing all six models it's clear that the EasyEnsemble AdaBoost Classifier shows the best results with this dataset. This algorithm has a Balanced accuracy rate of 92%, a recall score of 89% for high-risk loans and 94% for low-risk loans, and a F1 score of 96%. This would be the recommended algorithm for this analysis. Overall, both ensemble learners outperformed the four resampling models, with all four of those models showing a balanced accuracy score of 65% or below and recall rates of 70% or below. 
