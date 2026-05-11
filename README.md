# Customer Churn Prediction Using Explainable AI

## An end-to-end machine learning project focused on predicting customer churn and identifying the key behavioral, contractual, and financial drivers behind customer attrition using Explainable AI (SHAP).

## 📌 Business Problem
Customer churn directly impacts revenue growth, customer acquisition costs, and long-term profitability. Businesses that can proactively identify high-risk customers are better positioned to improve retention, optimize customer experience, and reduce revenue leakage. This project builds a complete churn prediction pipeline using multiple machine learning models and explainable AI techniques to:

- Predict the likelihood of customer churn
- Compare model performance across algorithms
- Understand the factors driving churn behavior
- Generate actionable business recommendations

## 🎯 Business Objectives

- Perform exploratory churn analysis
- Build robust preprocessing pipelines
- Compare multiple machine learning models
- Evaluate predictive performance using classification metrics
- Apply SHAP explainability for model transparency
- Translate analytical findings into business recommendations


## 🏦: Data
Source: [Kaggle](https://www.kaggle.com/competitions/playground-series-s6e3/data?select=train.csv) – Predict Customer Churn

Dataset Features

The dataset includes a mix of:

- Customer demographics
- Subscription information
- Billing information
- Payment methods
- Service usage behavior

Example Features
- tenure
- Contract
- InternetService
- MonthlyCharges
- TotalCharges
- PaymentMethod

### Target Variable
Churn
Yes = 1
No = 0

## Project Workflow

## 🛠️ Tools & Technologies

| Category | Tools |
| :--- | :--- |
| Language | Python |
ML	Scikit-learn |     XGBoost, LightGBM
Visualization	|     Matplotlib, Seaborn
Explainability	|  SHAP
Data Processing	|   Pandas, NumPy
Notebook Environment | Jupyter Notebooks 

## Exploratory Data Analysis

Key analyses performed include:

- Churn distribution analysis
- Churn by contract type
- Churn by payment method
- Churn by internet service
- Monthly charges vs churn
- Tenure distribution by churn
- Temporal churn patterns

## Machine Learning Models

The following models were developed and compared:

1. Logistic Regression

Baseline interpretable classification model.

2. Random Forest

Ensemble tree-based classifier for non-linear relationships.

3. XGBoost

Gradient boosting model optimized for predictive performance.

4. LightGBM

Efficient gradient boosting framework for scalable training.


## Data Preprocessing Pipeline

A production-style preprocessing pipeline was implemented using Scikit-learn.

### Numerical Features
- Standard scaling
### Categorical Features
- One-hot encoding
### Pipeline Components
- ColumnTransformer
- Pipeline
- SimpleImputer
- StandardScaler
- OneHotEncoder


## Model Evaluation

Models were evaluated using:
-Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

## Explainable AI with SHAP

SHAP (SHapley Additive exPlanations) was used to interpret model predictions and identify the primary drivers of customer churn.
### Explainability Visualizations
- SHAP Feature Importance Plot
- SHAP Beeswarm Plot
- SHAP Dependence Plot
- SHAP Waterfall Plot

## 📓 Key Insights
1. Customer Tenure is the Strongest Churn Driver

Customers with shorter tenure exhibit significantly higher churn probability.

2. Month-to-Month Contracts Increase Churn Risk

Flexible contract structures are strongly associated with customer attrition.

3. High Monthly Charges Correlate with Churn

Customers with higher recurring charges demonstrate elevated churn behavior.

4. Payment Behavior Matters

Electronic payment users showed higher churn likelihood compared to auto-payment customers.


## Business Recommendations

#### Improve Early Customer Retention

Develop onboarding and engagement programs targeting new customers during the first months of service.

#### Encourage Long-Term Contracts

Offer incentives for customers to migrate from month-to-month contracts to longer-term subscription plans.

#### Optimize Pricing Strategy

Evaluate pricing fairness and bundled offers for high-charge customer segments.

#### Deploy Proactive Retention Campaigns

Use churn prediction scores to trigger early intervention strategies for high-risk customers.


## SHAP Insights
#### SHAP Feature Importance

Identifies the features with the greatest impact on churn prediction.

### SHAP Beeswarm Plot

Shows how high and low feature values influence churn probability across customers.

### SHAP Waterfall Plot

Explains individual customer-level churn predictions.

## How to Run the Project

Clone Repository
```

git clone https://github.com/kurves/Customer-Churn-Prediction-Engine
```

Install Dependencies
```
pip install -r requirements.txt
```
Launch Jupyter Notebook
```
jupyter notebook
```
