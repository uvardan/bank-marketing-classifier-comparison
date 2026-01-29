# Bank Marketing Classifier Comparison

## Overview
This project compares four classifiers (KNN, Logistic Regression, Decision Tree, and SVM) on the Bank Marketing dataset to predict whether a client will subscribe to a term deposit (`y`).

## Business Objective
Use client profile information to predict subscription likelihood so marketing outreach can be better targeted and more efficient.

## Data & Features
- Dataset: `bank-additional-full.csv`
- Target: `y` (yes/no → 1/0)
- Features used for modeling (bank client info only): `age`, `job`, `marital`, `education`, `default`, `housing`, `loan`
- Excluded: `duration` (not available before the call; benchmark-only per dataset notes)
- Encoding: One-hot encoding for categorical features; scaling for `age`

## Baseline
Majority-class baseline accuracy (always predict “no”): **~0.887**

## Model Comparison (Default Settings + Class Weighting Where Supported)
Accuracy alone is misleading due to class imbalance, so we focus on F1/Recall for the “yes” class.

(Insert your results table here — or summarize the top model and key metrics.)

## Hyperparameter Tuning
Used GridSearchCV with **F1 (yes)** as the scoring metric to tune model hyperparameters.
(Insert tuned results summary here.)

## Notebook
See the full analysis and code here:
- [`prompt_III.ipynb`](./prompt_III.ipynb)

