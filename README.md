# Credit_Risk_Analysis
Supervised Machine Learning

## Overview

The purpose of this project was to apply machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, this project required employing different techniques to train and evaluate models with unbalanced classes; and using the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, data was oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled using the ClusterCentroids algorithm. Then, used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, two new machine learning models that reduce bias were compared - BalancedRandomForestClassifier and EasyEnsembleClassifier - to predict credit risk. 

## Results

### Oversampling

#### Naive Random Oversampling

In the naive random oversampling algorithm, the calculated balanced accuracy score was **64.03%**, the precision score for high_risk loans was **1%** and  sensitivity was **66%**. Due to the pronounced imbalance between precision and mean, a low F1 was derived at **2%**. 

<p align=center> <img src="https://user-images.githubusercontent.com/95978097/167976282-0ccd648a-80f0-497b-9cf4-d1ad7e2689a1.png"></p>

#### SMOTE Oversampling

In te SMOTE oversampling algorithm, the calculated balanced accuracy score was slightly higher at **65.15%** than that of naive random oversampling. The precision score for high_risk loans was **1%**, recall was **61%**, and again derived a low F1 score equal to **2%**.

<p align=center> <img src="https://user-images.githubusercontent.com/95978097/167981080-725c5a55-94bf-46f9-8189-96883bffd134.png"></p>

## Summary

