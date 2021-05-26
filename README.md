# Risky Business

![Risky_Business](02-Homework_11-Machine-Learning_Instructions_Images_credit-risk.PNG)


## Background

Auto loans, mortgages, student loans, debt consolidation ... these are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk, so you have been asked by a client to help them use machine learning techniques to predict credit risk.

I have built and evaluated several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so I have used different techniques for training and evaluating models with imbalanced classes, utilizing the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:

1. Resampling
2. Ensemble-Learning


## Prerequisites
numpy
pandas
pathlib
sklearn
collections
imblearn


## Resampling
I used the imbalanced learn library to resample the LendingClub data and build and evaluate logistic regression classifiers using the resampled data. then:

1. Oversample the data using the Naive Random Oversampler and SMOTE algorithms.
2. Undersample the data using the Cluster Centroids algorithm.
3. Over- and under-sample using a combination SMOTEENN algorithm.

For each of the above, I :

1. Trained a logistic regression classifier from sklearn.linear_model using the resampled data.
2. Calculated the balanced accuracy score from sklearn.metrics.
3. Calculated the confusion matrix from sklearn.metrics.
4. Printed the imbalanced classification report from imblearn.metrics.


## Ensemble Learning
In this section, I trained and compared two different ensemble classifiers to predict loan risk and evaluate each model. I used the balanced random forest classifier and the easy ensemble AdaBoost classifier.

for each model, I:

Trained the model using the quarterly data from LendingClub provided in the Resource folder.
Calculated the balanced accuracy score from sklearn.metrics.
Printed the confusion matrix from sklearn.metrics.
Generated a classification report using the imbalanced_classification_report from imbalanced learn.
For the balanced random forest classifier only, printed the feature importance sorted in descending order (most important feature to least important) along with the feature score.


## Built With
Python