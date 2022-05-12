# Credit_Risk_Analysis
Supervised Machine Learning

## Overview

The purpose of this project was to apply machine learning to solve a real-world challenge: credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, this project required employing different techniques to train and evaluate models with unbalanced classes; and using the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, data was oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled using the ClusterCentroids algorithm. Then, used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, two new machine learning models that reduce bias were compared - BalancedRandomForestClassifier and EasyEnsembleClassifier - to predict credit risk. 

## Results

### Oversampling

#### Naive Random Oversampling

In the naive random oversampling algorithm, the calculated balanced accuracy score was **64.03%**, the precision score for high_risk loans was **1%** and  sensitivity was **66%**. Due to the pronounced imbalance between precision and mean, a low F1 was derived at **2%**. 

<p align=center> <img src="https://user-images.githubusercontent.com/95978097/167981277-9fe24632-9ab4-4d3e-baf0-98e3bf5b7cb5.png"></p>

#### SMOTE Oversampling

In the SMOTE oversampling algorithm, the calculated balanced accuracy score was slightly higher at **65.15%** than that of naive random oversampling. The precision score for high_risk loans was **1%**, recall was **61%**, and again derived a low F1 score equal to **2%**.

<p align=center> <img src="https://user-images.githubusercontent.com/95978097/167981210-360d7490-1a8b-45c8-a701-820010400b1d.png"></p>

### Undersampling

When using the undersampling algorithm, the balanced accuracy score equated to **54.43%**. The high_risk precision score was again was **1%**, the recall score was **69%**, with a low F1 of **1%**.

<p align=center> <img src="https://user-images.githubusercontent.com/95978097/167981594-6cfc11bb-0b97-4136-a4b7-837cf9f6b9eb.png"></p>

### Combination (Over and Under) Sampling

In the combination sampling algorithm, the balanced accuracy score was **65.5%**, the high_risk precision was **1%**, recall was **72%**, and the F1 was **2%**.

<p align=center> <img src="https://user-images.githubusercontent.com/95978097/167981961-1aa7f0f0-ae19-445b-8ac2-7344af715ae3.png"></p>

## Summary

