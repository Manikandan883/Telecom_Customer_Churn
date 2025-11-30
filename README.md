Customer Churn Prediction – Machine Learning Project 

This project predicts telecom customer churn using Machine Learning models.
It includes EDA, statistics, feature engineering, modeling, tuning, and insights — everything required for a professional data science portfolio project.

 1. Project Objective

To identify customers who are likely to churn and provide business insights to help the telecom company reduce customer loss.

2. Data Preprocessing

Removed missing values from TotalCharges

Converted TotalCharges → numeric

Converted categorical variables using one-hot encoding

Train-test split using stratified sampling

Handled imbalance using class_weight='balanced'

3. Exploratory Data Analysis (EDA) — Key Findings

Month-to-month contract customers churn the most

Fiber optic users have higher churn

Electronic check payment method has highest churn

Customers with OnlineSecurity, TechSupport, OnlineBackup churn less

Higher MonthlyCharges → higher churn

Lower tenure → higher churn

 4. Statistical Validation (✔ Professional Touch)
Chi-square Tests (Categorical vs Churn):

Strong associations found with:

Contract

InternetService

OnlineSecurity

TechSupport

PaymentMethod

PaperlessBilling

Partner & Dependents

T-tests (Numeric vs Churn):
Feature	p-value	Meaning
Tenure	2.3e-234	Churn customers have very low tenure
MonthlyCharges	2.6e-72	Churn customers pay more
TotalCharges	1.15e-75	Churners have low total charges
5. Feature Engineering

Dropped customerID

One-hot encoding for categorical variables

Balanced training using class weights

Train-test split with 80/20 ratio

6. Machine Learning Models Built
 
 * Logistic Regression

       Accuracy: 73%
       
       Recall (Churn): 80%
       
       F1-score (Churn): 0.61

* Random Forest (Base Model)

       Accuracy: 79%
       
       Precision (Churn): 63%
       
       Recall (Churn): 50%
     
* Tuned Random Forest (Best Model) 

       Accuracy: 76%
       
       Recall (Churn): 75%
       
       Precision (Churn): 53%
       
       F1-score (Churn): 0.62

This model correctly identifies 3 out of 4 churners — best for business use.

 *  XGBoost

        Accuracy: 75%
        
        Recall (Churn): 73%
        
        F1-score (Churn): 0.61


7 Final Feature Importance (From Best Model – Tuned RF)

Top churn drivers:

TotalCharges

Tenure

MonthlyCharges

Contract (Month-to-Month vs Others)

Fiber Optic Internet

Electronic Check Payment

OnlineSecurity

TechSupport

PaperlessBilling

SeniorCitizen

 8. Business Recommendations

Offer retention discounts for high monthly charge customers

Convert month-to-month users into 1–2 year contracts

Improve fiber optic service quality

Educate customers to switch from electronic check to autopay/card

Give early engagement benefits to new customers (low tenure)

Promote OnlineSecurity + TechSupport bundles to reduce churn

9. Conclusion

The project successfully built an end-to-end churn prediction system.
Tuned Random Forest achieved the highest recall and balanced performance, making it ideal for churn detection.

This project includes:

EDA

Feature engineering

Statistical analysis

Modeling

Hyperparameter tuning

Business insights

Perfect for real-world telecom churn prevention.
