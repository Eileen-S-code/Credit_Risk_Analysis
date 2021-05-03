# Credit Risk Analysis

## Overview of the analysis: 
Credit risk is an inherently unbalanced classification problem therefore different techniques were employed to train and evaluate models with unbalanced classes. Using the credit card credit dataset from LendingClub, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Then two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, were to predict credit risk. 

## Results: 
The native random sampler was 64% accurate 
![Native random sampler](https://user-images.githubusercontent.com/75797531/116833273-f71bfb80-ab7d-11eb-9a77-789ec0c7406a.PNG)

The SMOTE Oversampling is 66% accurate 
![Smote oversampler](https://user-images.githubusercontent.com/75797531/116833370-5974fc00-ab7e-11eb-9bfa-e802206d6995.PNG)

The undersampler was 54% accurate
![undersample](https://user-images.githubusercontent.com/75797531/116833394-76a9ca80-ab7e-11eb-8f92-0b5c264b2642.PNG)

The Combination sampler was 64% accurate
![over and under](https://user-images.githubusercontent.com/75797531/116833410-97722000-ab7e-11eb-89a5-8a6466e9a890.PNG)


The Random Forest sampler was 78% accurate
![random forest](https://user-images.githubusercontent.com/75797531/116833429-bcff2980-ab7e-11eb-8933-c8ba073bb821.PNG)

The Easy Ensemble was 93% acccurate
![easy ensamble](https://user-images.githubusercontent.com/75797531/116833472-e6b85080-ab7e-11eb-8225-2228d3bc128e.PNG)

## Summary: 
The first models tested the difference between oversampling, undersampling, and then a combination of undersampling and oversampling. The next to models resampled the data and utilized ensemble classiffiers. I would recommend the Easy Ensemble as it has the best accuracy. 
