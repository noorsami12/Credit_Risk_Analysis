# Credit_Risk_Analysis

## Overview of the Analysis

The purpose of this analysis was to employ various strategies to train and evaluate models with unbalanced classes in order to analyze credit card risk. I used a credit card credit dataset and oversampled the data with RandomOverSampler and SMOTE, then undersampled the data with ClusterCentroids. I compared further learning models that reduce bias (BalancedRandomForestClassifier and EasyEnsembleClassifier), and at the end, I evaluated the performance of all the models to recommend whether they should be used to predict credit risk or not.

## Results

- Oversampling using RandomOverSampler resulted in a balanced accuracy score of .66, a precision of .99, and a recall of .60.
- Oversampling using SMOTE resulted in a balanced accuracy score of .66, a precision of .99, and a recall of .69.
- Undersampling using ClusterCentroids resulted in a balanced accuracy score of .54, a precision of .99, and a recall of .40.
- Combination over and under sampling using SMOTEENN resulted in a balanced accuracy score of .66, a precision of .99, and a recall of .54.
- Resampling using BalancedRandomForestClassifier resulted in a balanced accuracy score of .79, a precision of .99, and a recall of .87.
- Resampling using EasyEnsembleClassifier resulted in a balanced accuracy score of .93, a precision of .99, and a recall of .94.

![oversampling1](https://github.com/noorsami12/Credit_Risk_Analysis/blob/c7a7f4e7c763bbe848d8c8aafb3dcea8ee390730/oversampling1.png)
![oversampling2](https://github.com/noorsami12/Credit_Risk_Analysis/blob/c7a7f4e7c763bbe848d8c8aafb3dcea8ee390730/oversampling2.png)
![undersampling](https://github.com/noorsami12/Credit_Risk_Analysis/blob/c7a7f4e7c763bbe848d8c8aafb3dcea8ee390730/undersampling.png)
![combination](https://github.com/noorsami12/Credit_Risk_Analysis/blob/c7a7f4e7c763bbe848d8c8aafb3dcea8ee390730/combination.png)
![resampling1](https://github.com/noorsami12/Credit_Risk_Analysis/blob/c7a7f4e7c763bbe848d8c8aafb3dcea8ee390730/resampling1.png)
![resampling2](https://github.com/noorsami12/Credit_Risk_Analysis/blob/c7a7f4e7c763bbe848d8c8aafb3dcea8ee390730/resampling2.png)

## Summary

Ultimately, the models using BalancedRandomForestClassifier and EasyEnsembleClassifier has the greatest balanced accuracy and recall. I would recommend using the EasyEnsembleClassifier to predict credit risk due to its high balanced accuracy score at .93, as well as its high precision of .99 and recall of .94. I would not recommend undersampling, oversampling, or doing a combination, as all three models had very low balanced accuracy scores, with undersampling being the lowest at .54.

