**Customer Churn Prediction - California Telecom Case Study**

**Overview**
This project focuses on analyzing customer churn behaviour for a California-based telecommunication company. Using data exploration and machine learning techniques, we aim to predict customer churn and identify key contributing factors. The insights from this analysis can help the company implement better customer retention strategies.

**Dataset**
The dataset is sourced from Kaggle (originally scraped from Maven Analytics) and contains 7043 observations with 38 features. It includes customer demographic details, subscription services, tenure, billing information, and churn status.

**Project Components:**

1. Exploratory Data Analysis (EDA)

Data cleaning and handling missing values
Visualizing churn patterns
Statistical analysis to identify key churn factors

2. Feature Engineering

Creating new features like year_tenure and age_group
Performing feature selection using ANOVA and chi-square tests
Encoding categorical features using label encoding and binary encoding

3. Machine Learning Model

Model: Random Forest Classifier
Data Balancing Techniques: SMOTE, SMOTEENN
Hyperparameter tuning and cross-validation

4. Evaluation Metrics

Accuracy: 97.11%
Confusion Matrix
ROC Curve Analysis
Focus on minimizing False Negatives (Type II Error)

**Findings**

High-risk Customers: Recent customers (<1-year tenure) with high monthly charges
Contract Influence: Month-to-month customers have a high churn rate (~52%)
Offer Effectiveness: Offer A retains customers better, while Offer E has a high churn rate (~68%)
Revenue Impact: Churned customers contributed 17.28% of the total revenue
**
Future Work**

Incorporating customer satisfaction surveys
Using advanced sampling techniques for better data balancing
Implementing a recommendation system to reduce churn
