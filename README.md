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
- Code can be found at [Credit_Risk_Ensemble](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb) and [Credit_Risk_Resampling](https://github.com/pfrivas/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb)


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

**SMOTE Model Results Overview**
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

### Overall Summary of the Results

When all six models were ran and compared, the EasyEnsembleClassifier model produced the best results with 93% accuracy and 7% precision when predicting high risk candidates. The ClusterCentroids model produced the worst results with 54% accuracy and 1% precision when predicting high risk candidates.


- **Ranking of models in descending order based on "High Risk" results:**
  - ***EasyEnsembleClassifier Model***
    - 93% Accuracy
    - 7% precision
    - 91% Recall
    - 14% F1 Score
  - ***BalancedRandomForestClassifier Model***
    - 79% Accuracy
    - 4% precision
    - 67% Recall
    - 7% F1 Score
  - ***SMOTE Model***
    - 66% Accuracy
    - 1% precision
    - 63% Recall
    - 2% F1 Score
  - ***RandomOverSampler Model***
    - 65% Accuracy
    - 1% precision
    - 72% Recall
    - 2% F1 Score
  - ***SMOTEENN Model***
    - 65% Accuracy
    - 1% precision
    - 72% Recall
    - 2% F1 Score
  - ***ClusterCentroids Model***
    - 54% Accuracy
    - 1% precision
    - 69% Recall
    - 1% F1 Score

### Recommendation on which Model to use

Unfortunately all models have a very low precision with the highest precision being 7% in the EasyEnsembleClassifier Model. With a low precision there could be a lot of false positives for high risk candidates. For that reason, none of these models should be used when predicting credit risk in candidates. However, if the bank did have to choose one of these six models to use, then the EasyEnsembleClassifier Model would be the most accurate (97% accuracy) and precise (7% precision) model to use in predicting credit risk in potential candidates.
