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

### SMOTE Model

**Balanced Accuracy Score**

- ![smote_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Model/SMOTE_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![smote_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Model/SMOTE_ConfusionMatrix.png)

- ![smote_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Model/SMOTE_ICR.png)



### ClusterCentroids Model

**Balanced Accuracy Score**

- ![cc_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids%20Model/ClusterCentroids_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![cc_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids%20Model/ClusterCentroids_ConfusionMatrix.png)

- ![cc_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids%20Model/ClusterCentroids_ICR.png)


### SMOTEENN Model

**Balanced Accuracy Score**

- ![smote_enn_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTEENN%20Model/SMOTEEN_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![smote_enn_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTEENN%20Model/SMOTEEN_ConfusionMatrix.png)

- ![smote_enn_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/SMOTEENN%20Model/SMOTEEN_ICR.png)


### BalancedRandomForestClassifier Model 

**Balanced Accuracy Score**

- ![brfc_bac](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForest%20Classifier%20Model/RandomForest_BalancedAccuracyScore.png)

**Precision and Recall Scores**

- ![brfc_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForest%20Classifier%20Model/RandomForest_ConfusionMatrix.png)

- ![brfc_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForest%20Classifier%20Model/RandomForest_ICR.png)


### EasyEnsembleClassifier Model

**Balanced Accuracy Score**

- ![eec_bac](https://github.com/pfrivas/Credit_Risk_Analysis/tree/main/Images/EasyEnsembleClassifier%20Model)

**Precision and Recall Scores**

- ![eec_cm](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier%20Model/EEC_ConfusionMatrix.png)

- ![eec_icr](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/Images/EasyEnsembleClassifier%20Model/EEC_ICR.png)



## Summary:

### Summary of the Results
**Ranking of models in descending order based on "High Risk" results:**
-
-
-
-
-
-

### Recommendation on which Model to use
