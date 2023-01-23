# Credit_Risk_Analysis

## Overview of the Loan Prediction Risk Analysis:

### Purpose

The purpose of this analysis is to build and evaluate various machine learning models to evaluate individual customer credit risk. This was done by employing different techniques to train and evaluate models with unbalanced classes, as well as using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the data was oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled using the ClusterCentroids algorithm. Then using a combinatorial approach of over- and undersampling the SMOTEENN algorithm was used. Next, two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, were used to predict credit risk. 

**Overall the machine learning algorithms used were:**
- RandomOverSampler
- SMOTE
- ClusterCentroids
- SMOTEENN
- BalancedRandomForestClassifier
- EasyEnsembleClassifier

### Resources
- Data Source: LendingClub (LoanStats_2019Q1)
- Software: Python, Anaconda, and Jupyter Notebooks


## Results:

### RandomOverSampler Model

**Balanced Accuracy Score**

- ![roc_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/RandomOversampler%20Model/RandomOverSampler_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![roc_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/RandomOversampler%20Model/RandomOverSampler_ConfusionMatrix.png)

- ![roc_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/RandomOversampler%20Model/RandomOversampler_ICR.png)

**RandomOverSampler Model Results Overview**
- Balanced accuracy score: 65.47%.
- The "High Risk" precision rate was only 1% with the recall at 72% giving this model an F1 score of 2%.
- The "Low Risk" had a precision rate of 100% and recall at 59%.


### SMOTE Model

**Balanced Accuracy Score**

- ![smote_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Model/SMOTE_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![smote_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Model/SMOTE_ConfusionMatrix.png)

- ![smote_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Model/SMOTE_ICR.png)

**SMOTEE Model Results Overview**
- Balanced accuracy score: 66.20%.
- The "High Risk" precision rate was only 1% with the recall at 63% giving this model an F1 score of 2%.
- The "Low Risk" had a precision rate of 100% and recall at 69%.



### ClusterCentroids Model

**Balanced Accuracy Score**

- ![cc_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids%20Model/ClusterCentroids_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![cc_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids%20Model/ClusterCentroids_ConfusionMatrix.png)

- ![cc_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids%20Model/ClusterCentroids_ICR.png)

**ClusterCentroids Model Results Overview**
- Balanced accuracy score: 54.42%.
- The "High Risk" precision rate was only 1% with the recall at 69% giving this model an F1 score of 1%.
- The "Low Risk" had a precision rate of 100% and recall at 40%.


### SMOTEENN Model

**Balanced Accuracy Score**

- ![smote_enn_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTEENN%20Model/SMOTEEN_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![smote_enn_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTEENN%20Model/SMOTEEN_ConfusionMatrix.png)

- ![smote_enn_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTEENN%20Model/SMOTEEN_ICR.png)

**SMOTEENN Model Results Overview**
- Balanced accuracy score: 64.73%.
- The "High Risk" precision rate was only 1% with the recall at 72% giving this model an F1 score of 2%.
- The "Low Risk" had a precision rate of 100% and recall at 57%.


### BalancedRandomForestClassifier Model 

**Balanced Accuracy Score**

- ![brfc_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForest%20Classifier%20Model/RandomForest_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![brfc_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForest%20Classifier%20Model/RandomForest_ConfusionMatrix.png)

- ![brfc_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForest%20Classifier%20Model/RandomForest_ICR.png)

**BalancedRandomForestClassifier Model Results Overview**
- Balanced accuracy score: 78.78%.
- The "High Risk" precision rate was only 4% with the recall at 67% giving this model an F1 score of 7%.
- The "Low Risk" had a precision rate of 100% and recall at 91%.


### EasyEnsembleClassifier Model

**Balanced Accuracy Score**

- ![eec_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier%20Model/EEC_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![eec_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier%20Model/EEC_ConfusionMatrix.png)

- ![eec_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier%20Model/EEC_ICR.png)

**EasyEnsembleClassier Model Results Overview**
- Balanced accuracy score: 92.54%.
- The "High Risk" precision rate was only 7% with the recall at 91% giving this model an F1 score of 14%.
- The "Low Risk" had a precision rate of 100% and recall at 94%.


## Summary:

### Summary of the Results
- **Ranking of models in descending order based on "High Risk" results:**
  - EasyEnsembleClassifier Model
    - 92.54% Accuracy
    - 7% precision
    - 91% Recall
    - 14% F1 Score
  - BalancedRandomForestClassifier Model
  - SMOTE Model
  - RandomOverSampler Model
  - SMOTEENN Model
  - ClusterCentroids Model

### Recommendation on which Model to use
