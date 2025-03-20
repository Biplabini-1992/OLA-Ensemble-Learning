# OLA-Ensemble-Learning
## Objective:
This project focuses on predicting driver attrition for Ola using historical data on driver demographics, tenure, performance, and income. The goal is to help Ola reduce churn, retain drivers, and optimize acquisition costs.



## Key Steps:

  ### 1. Data Preprocessing & Feature Engineering:
    - Convert date-like features to appropriate format
    - Handle missing values using KNN Imputation
    - Aggregate data to remove duplicate driver records
    - Create new features:
        - Quarterly Rating Change Flag: 1 if increased
        - Monthly Income Change Flag: 1 if increased
        - Attrition Flag: 1 if driver has left
    - One-hot encoding of categorical variables
    - Standardization of numerical features
  
  ### 2. Model Building:
    - Handling Class Imbalance using oversampling/undersampling techniques
    - Ensemble Learning: Implementing Bagging (Random Forest) and Boosting (XGBoost, LightGBM)
    - Hyperparameter tuning for model optimization
  
  ### 3. Model Evaluation:
    - Classification Report (Precision, Recall, F1-Score, Accuracy)
    - ROC-AUC Curve
  ### 4. Business Insights & Recommendations:
    - Identify key factors influencing driver attrition
    - Suggest strategies to improve driver retention and optimize hiring
    - Data-driven approach to reducing acquisition costs
