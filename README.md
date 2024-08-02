# Churn Analysis Project

This repository contains a sample project for analyzing customer churn in a subscription service. The project uses Python for data analysis and model building, and Tableau for data visualization.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Building](#model-building)
- [Evaluation](#evaluation)
- [Tableau Visualizations](#tableau-visualizations)

## Project Overview

The goal of this project is to predict customer churn for a subscription service. The analysis involves:

1. Data Preprocessing
2. Exploratory Data Analysis (EDA)
3. Model Building and Training
4. Model Evaluation
5. Exporting Data for Tableau Visualization

## Dataset

The dataset used for this project is synthetically generated and consists of the following features:

- `CustomerID`: Unique identifier for each customer
- `Gender`: Gender of the customer
- `Age`: Age of the customer
- `Tenure`: Number of months the customer has been with the company
- `SubscriptionPlan`: Subscription plan of the customer (Basic, Standard, Premium)
- `MonthlyCharges`: Monthly charges for the customer
- `Churn`: Whether the customer has churned (0 = No churn, 1 = Churn)
- `TotalCharges`: Total charges for the customer (calculated as `Tenure` * `MonthlyCharges`)


## Exploratory Data Analysis (EDA)

The EDA section of the code includes:

- **Churn Count Visualization**: This plot shows the distribution of churned vs. non-churned customers, providing a quick look at the imbalance in the dataset.
- **Age Distribution Visualization**: A histogram that displays the age distribution of customers, helping to understand the age range and common age groups within the dataset.
- **Monthly Charges by Subscription Plan Visualization**: A box plot that illustrates the distribution of monthly charges across different subscription plans, highlighting the variations in charges among the plans.
- **Correlation Matrix Visualization**: A heatmap showing the correlation between different numerical features, which helps in identifying the relationships and dependencies among the features.

## Model Building

The model building process includes:

- Train-test split with stratification
- Feature scaling
- Training a RandomForestClassifier

## Evaluation

The model evaluation includes:

- **Classification Report**: Provides precision, recall, and F1-score for the model, giving a detailed performance summary.
- **Confusion Matrix**: A matrix that shows the counts of true positives, true negatives, false positives, and false negatives, helping to evaluate the classification accuracy.
- **ROC AUC Score**: The ROC AUC score is used to measure the model's ability to distinguish between classes.
- **ROC Curve Visualization**: A plot of the True Positive Rate (TPR) against the False Positive Rate (FPR), showing the performance of the classification model at various threshold settings.
- **Feature Importance Visualization**: A bar plot that ranks the features based on their importance in the model, indicating which features have the most influence on predicting churn.

## Tableau Visualizations

You can view the Tableau visualizations for this project [here](https://public.tableau.com/views/ChurnAnalysisDashboard_17225321250850/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

---