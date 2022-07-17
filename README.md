# Credit Risk Analysis

## Overview

The purpose of this project is to use machine learning to help evaluate credit card risk using a file of loan applications and their statuses and evaluate which model works best on such an imbalanced dataset. The data needs to be balanced to achieve reliable results and will use oversampling with the RandomOverSampler and SMOTE algorithms, undersampling with the ClusterCentroids algorithm, and a combo approach of over and undersampling with the SMOTEENN algorithm. Two bias reduction algorithims are then compared, BalancedRandomForestClassifier and EasyEnsemble AdaBoost algorithms. The balanced accuracy scores and precision and recall scores will be used to compare the six algorithms. 

## Resources

- Data: LoanStats_2019Q1.csv
- Software: Jupyter Notebook 6.4.8; Python 3.7.13; Imbalanced-Learn Library 0.9.0; SciKit-Learn Library 1.0.2

## Results

### RandomOverSampler Model

!
