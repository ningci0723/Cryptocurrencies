# Credit Risk Analysis

## Overview

For this project, we will use the credit card credit dataset from LendingClub, a peer-to-peer lending services company, oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm.Then we will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Finally, we will ompare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.


## Results

1. Random OverSampling Model
![RandomOverSampler model](https://github.com/ningci0723/Credit_Risk_Analysis/blob/main/Images/RandomOverSampler.png)

The model classified 51366 records each as High Risk and Low Risk.
* The balanced accuracy score is 65%.
* The precision is low for high-risk loans and its almost 100% for low-risk loans.
* The "High Risk" precision rate was only 1% with the recall at 72% giving this model an F1 score of 2%.
* "Low Risk" had a precision rate of 100% and recall at 59%.

2. SMOTE Oversampling Model
![SMOTE Oversampling model](https://github.com/ningci0723/Credit_Risk_Analysis/blob/main/Images/SMOTE%20Oversampling%20model.png)

The model classified 51366 records each as High Risk and Low Risk. The result is similar to the RandomOverSampling model.
* The balanced accuracy score is 65%.
* The precision is low for high-risk loans and its almost 100% for low-risk loans.
* The "High Risk" precision rate was only 1% with the recall at 72% giving this model an F1 score of 2%.
* "Low Risk" had a precision rate of 100% and recall at 59%.

3. Undersampling Model
![Undersamplig model](https://github.com/ningci0723/Credit_Risk_Analysis/blob/main/Images/Undersampling.png)

The model classified 246 records each as High Risk and Low Risk.
* The balanced accuracy score is down to 52%.
* The precision is low for high-risk loans and its almost 100% for low-risk loans.
* The "High Risk" precision rate was only 1% with the recall at 69% giving this model an F1 score of 2%.
* "Low Risk" had a precision rate of 100% and recall at 40%.

4. SMOTEENN Model
![Combined model](https://github.com/ningci0723/Credit_Risk_Analysis/blob/main/Images/Combined%20.png)

* The balanced accuracy score is 64%.
* The precision is low for high-risk loans and its almost 100% for low-risk loans.
* The "High Risk" precision rate was only 1% with the recall at 72% giving this model an F1 score of 2%.
* "Low Risk" had a precision rate of 100% and recall at 57%.

5. Balanced Random Forest Classifier Model
![Balanced Random Forest Classifier Model](https://github.com/ningci0723/Credit_Risk_Analysis/blob/main/Images/Balanced%20Random%20Forest%20Classifier%20Model.png)

* The balanced accuracy score is 78%.
* The precision is low for high-risk loans and its almost 100% for low-risk loans.
* The "High Risk" precision rate was 3% with the recall at 70% giving this model an F1 score of 6%.
* "Low Risk" had a precision rate of 100% and recall at 87%.

6. Easy Ensemble AdaBoost Classifier Model
![Easy Ensemble AdaBoost Classifier Model](https://github.com/ningci0723/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20AdaBoost%20Classifier%20Model.png)

* The balanced accuracy score is 93%.
* The precision is low for high-risk loans and its almost 100% for low-risk loans.
* The "High Risk" precision rate was 9% with the recall at 92% giving this model an F1 score of 16%.
* "Low Risk" had a precision rate of 100% and recall at 94%.


## Summary
In reviewing all these models, the Easy Ensemble AdaBoost Classifier Model shows the best results.The Ensemble models improved a lot specially on the sensitivity of the high risk credits. The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit. I would like to choose Easy Ensemble AdaBoost Classifier Model for further credit card analysis. 
On the other hand, if the credit risk is high, all the models which are used to perform the credit risk analysis show weak precision in determining.
