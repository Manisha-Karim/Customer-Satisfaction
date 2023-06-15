
# Customer Satisfaction

Santander Bank is asking Kagglers to help them identify dissatisfied customers early in their relationship. Doing so would allow Santander to take proactive steps to improve a customer's happiness before it's too late.

In this competition, you'll work with hundreds of anonymized features to predict if a customer is satisfied or dissatisfied with their banking experience.
# Dataset Description

## Dataset Source

The dataset was collected from Kaggle.

## Dataset Description

The dataset consisted of 76020 rows and 371 unnamed features.  The "TARGET" column is the variable to predict. It equals one for unsatisfied customers and 0 for satisfied customers.

## Feature Engineering

1. Features who had less than 2% variance were removed.

2. Features who were highly correlated(90%) were removed.

3. Features with minimal correlation(0.1%) with the target were also removed.

4. 59 most important features were selected using ExtraTreeClassifier

5. The final 16 features were selected using Recursive Feature Elimination, chi-squared test, and model based feature selection like Random Forest, Logistic Regression, Lightgbm


## Classifier

Three classifiers (KNN, DT, and RF) were fitted with hyperparameter tuning using GridSearchCV. All of them had an accuracy of 86% approximately.
