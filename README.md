# Customer Churn Prediction Using Mobile Game Activity Data

## Overview

This project predicts whether mobile game users are likely to become inactive based on their early activity patterns.

The goal is to transform raw user activity logs into user-level features and compare machine learning models for customer churn prediction.

## Business Problem

For many digital products, users do not formally cancel their accounts. Instead, they simply stop using the service.

This project uses early user behavior to identify users who may be at risk of churn.

## Dataset

The dataset contains mobile game activity logs, including user ID, timestamp, and game score.

The raw event-level data was aggregated into a user-level dataset for modeling.

## Method

Churn was defined based on whether a user was active in the first few days but inactive afterward.

Behavior-based features were created to capture user engagement, recency, activity frequency, active days, and score patterns.

## Models

Three classification models were compared:

- Logistic Regression
- Random Forest
- XGBoost

Class imbalance was handled during model training.

## Results

The models achieved similar overall performance, with ROC-AUC scores around 0.798.

Recent activity and number of active days were the strongest indicators of future user inactivity.

## Tools

- Python
- pandas
- NumPy
- scikit-learn
- XGBoost
- matplotlib
- seaborn

## Repository Structure

```text
.
├── data/              # Dataset file
├── notebooks/         # Data preparation, feature engineering, and modeling notebook
├── outputs/           # visualization outputs
└── README.md
````

