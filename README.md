# Optimizing Insurance Premiums with Predictive Claim Analysis

## Project Overview

This project focuses on predicting the probability of an insurance claim based on various policy and car safety features. The goal is to assist insurance companies in dynamically adjusting premiums based on the risk associated with policyholders, thereby improving customer satisfaction and reducing company losses.

## Table of Contents
1. [Problem Statement](#problem-statement)
2. [Objective](#objective)
3. [Data Overview](#data-overview)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Feature Engineering](#feature-engineering)
6. [Model Training and Evaluation](#model-training-and-evaluation)
7. [Significant Feature Contribution](#significant-feature-contribution)
8. [Conclusion](#conclusion)

## Problem Statement
Insurance companies struggle with accurately assessing the risk of claims, which can lead to suboptimal premium pricing. This project aims to create a predictive model to identify the likelihood of claims, helping insurers set appropriate premiums and manage risks more effectively.

## Objective
The objective is to develop a robust machine learning model that predicts if a policyholder will file a claim and identify the most influential factors affecting this likelihood.

## Data Overview
- **Total Records:** 58,592
- **Features:** 44, including both numerical and categorical data.
- **Target Variable:** `is_claim`, indicating whether a claim was filed.

## Exploratory Data Analysis
Initial data exploration revealed several key insights:
- Significant class imbalance, with a majority of policies having no claims.
- Skewed distributions in numerical features like `age_of_car` and `age_of_policyholder`.
- Certain categorical features, such as `area_cluster` and `model`, showed notable differences in claim rates.

## Feature Engineering
Key steps in feature engineering included:
- Handling outliers in continuous variables.
- Encoding categorical features using Label Encoding.
- Creating new features like `volume` from existing ones.
- Selecting the most informative features using Mutual Information.

## Model Training and Evaluation
Various models were trained using different sampling techniques:
- **SMOTENC** for oversampling the minority class.
- **Random Undersampling** to balance the classes by reducing the majority class size.

Tree-based models like Random Forest and XGBoost were selected for their robustness to feature scaling and their ability to handle mixed data types. Hyperparameter tuning was performed to improve model performance, focusing on metrics like recall and AUC.

### Best Model
The XGBoost classifier emerged as the best model with the following hyperparameters:
- `n_estimators=405`
- `max_depth=5`
- `learning_rate=0.037`
- `gamma=4.96`

Performance metrics:
- **Recall:** 0.74
- **Accuracy:** 0.51
- **AUC:** 0.67

![Metrics](https://github.com/user-attachments/assets/ad641837-493b-4334-9c27-986979433c79)


## Significant Feature Contribution
![KeyFeatures](https://github.com/user-attachments/assets/f73017d7-7464-462d-af2b-17628805bfe4)
Key features impacting the model's predictions include:
- `policy_tenure`
- `age_of_car`
- `area_cluster`
- `age_of_policyholder`


These features were crucial in determining the likelihood of claims.

## Conclusion
This project successfully developed a predictive model for insurance claims, leveraging significant features and robust machine-learning techniques. The XGBoost model, with fine-tuned hyperparameters, demonstrated strong performance in capturing the risk of claims, making it suitable for deployment in real-world insurance applications.


