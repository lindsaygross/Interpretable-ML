# Interpretable-ML: Telco Customer Churn Analysis

## Overview

This project investigates customer churn at a telecommunications company using interpretable machine learning models. The goal is to understand which factors contribute most to churn and to build predictive models that are both accurate and interpretable.


Dataset: https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data


## Project Structure


## Tasks

**1. Exploratory Data Analysis (EDA)**

- Investigate feature distributions and relationships with churn
- Use visualizations (e.g., boxplots, barplots, KDEs)
- Evaluate assumptions for:
Linear regression
Logistic regression
Generalized Additive Models (GAM)

**2. Linear Regression**
- Treat churn as a continuous variable (0 or 1)
- Fit a linear regression model
- Interpret coefficients and assess performance

**3. Logistic Regression**
- Treat churn as a binary classification problem
- Fit a logistic regression model
- Interpret model coefficients and log-odds

**4. Generalized Additive Model (GAM)**
- Fit a GAM to capture non-linear trends
- Visualize partial dependence plots
- Interpret smooth relationships

**5. Model Comparison & Recommendation**
- Compare linear, logistic, and GAM models on:
- Accuracy/performance
- Interpretability

Recommend best approach for the telecom company based on findings

## Models Used 
### Linear Regression:	
- Predict continuous churn probability	
- Assumes linearity
### Logistic Regression:
- Classify customers as churn/no churn	
- Probabilistic, interpretable
### GAM	
- Capture smooth, non-linear feature effects	
- More flexible but still interpretable


## How to Run 
1. Open Interpretable_ML.ipynb in Google Colab
2. Ensure WA_Fn-UseC_-Telco-Customer-Churn.csv is available in your environment
3. Run all cells in order
4. All necessary packages are listed in requirements.txt

## Dataest Descpriton 
Each row represents a customer with the following feauture:

- Demographic: Gender, SeniorCitizen, etc.

- Account info: Contract type, tenure, billing method

- Services: InternetService, OnlineBackup, TechSupport

- Target variable: Churn (Yes/No)

## Results
- **Linear Regression**: Accuracy ~0.73, ROC-AUC ~0.77 (not suitable for churn prediction).
- **Logistic Regression**: Accuracy ~0.80, ROC-AUC ~0.84 (best performing model).
- **GAM**: Accuracy ~0.77, ROC-AUC ~0.81 (slightly weaker performance but best interpretability).

**Recommendation**: Use Logistic Regression for churn prediction, and GAM for insights into customer behavior.


## Author
Lindsay Gross

MEng AI

AIPI 590: Explainable AI

