# Customer Churn Prediction - California Telecom Case Study  
**Predicting Customer Churn Using Machine Learning**

![Python](https://img.shields.io/badge/Python-3.8%2B-brightgreen) 

## 📌 Overview  
This project analyzes customer churn behavior for a California-based telecom company. Leveraging exploratory data analysis (EDA) and machine learning, identified drivers of churn and build a predictive model to enable proactive retention strategies. The model achieves **97.11% accuracy**, focusing on minimizing false negatives (high-risk churn customers).
## 📂 Dataset  
[Kaggle Dataset](https://www.kaggle.com/datasets/shilongzhuang/telecom-customer-churn-by-maven-analytics/data) (7,043 customers, 38 features)  
- **Features**: Demographics (age, gender), subscription details (contract type, internet service), billing (monthly charges, payment method), and churn status.  
- **Target Variable**: `Churn` (Yes/No).
## 🛠 Project Components  

### 1. Exploratory Data Analysis (EDA)  
- Handled missing values in `TotalCharges` by median imputation.  
- Visualized churn patterns:  
  - 52% churn rate for month-to-month contracts.  
  - 68% churn rate for customers under "Offer E".  
- Identified high-risk segments: Customers with <1-year tenure and high monthly charges.

### 2. Feature Engineering  
- Created new features:  
  - `year_tenure`: Tenure converted to years.  
  - `age_group`: Binned customer age into categories (e.g., 18-25, 26-35).  
- Selected top 15 features using ANOVA (numerical) and chi-square (categorical).  
- Encoded categorical variables with label/binary encoding.

### 3. Machine Learning Model  
- **Algorithm**: Random Forest Classifier.  
- **Balancing Techniques**:  
  - **SMOTE**: Oversampled minority class (churn=Yes).  
  - **SMOTEENN**: Combined oversampling and undersampling.  
- **Hyperparameter Tuning**: Optimized using grid search (5-fold cross-validation).
  
### 4. Evaluation Metrics  
| Metric          | Value   |
|-----------------|---------|
| Accuracy        | 97.11%  |
| Precision       | 0.97    |
| Recall          | 0.95    |
| ROC-AUC Score   | 0.98    |

- **Confusion Matrix**: Prioritized reducing false negatives (Type II errors).  
- **Key Insight**: Churned customers contributed 17.28% of the total revenue.
## 🔍 Key Findings  
- **Contract Type**: Month-to-month customers are 3x more likely to churn than those on annual contracts.  
- **Offers**: Offer A reduced churn by 22%, while Offer E increased churn risk by 68%.  
- **Tenure**: 60% of churn occurred within the first year of subscription.




