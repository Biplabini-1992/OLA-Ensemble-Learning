# OLA-Ensemble-Learning
- Recruiting and retaining drivers is seen by industry watchers as a tough battle for Ola. Churn among drivers is high and it’s very easy for drivers to stop working for the service on the fly or jump to Uber depending on the rates.

- As the companies get bigger, the high churn could become a bigger problem. To find new drivers, Ola is casting a wide net, including people who don’t have cars for jobs. But this acquisition is really costly. Losing drivers frequently impacts the morale of the organization and acquiring new drivers is more expensive than retaining existing ones.

- Therefore, identifying the key factors contributing to driver attrition and developing predictive models to foresee and address potential departures is imperative for sustaining growth and competitive advantage.

## Objective:
The objective of this analysis is to develop a predictive model to determine the likelihood of a driver leaving Ola based on various attributes. The data provided encompasses monthly information for a segment of drivers for the years 2019 and 2020, including:
  
  - Demographics: City, age, gender, etc.
  - Tenure Information: Joining date, last date.
  - Performance History: Quarterly ratings, monthly business acquired, grade, income.

## Dataset Information:
The dataset has following features.
  - MMMM-YY : Reporting Date (Monthly)
  - Driver_ID : Unique id for drivers
  - Age : Age of the driver
  - Gender : Gender of the driver – Male : 0, Female: 1
  - City : City Code of the driver
  - Education_Level : Education level – 0 for 10+ ,1 for 12+ ,2 for graduate
  - Income : Monthly average Income of the driver
  - Date Of Joining : Joining date for the driver
  - LastWorkingDate : Last date of working for the driver
  - Joining Designation : Designation of the driver at the time of joining
  - Grade : Grade of the driver at the time of reporting
  - Total Business Value : The total business value acquired by the driver in a month (negative business indicates cancellation/refund or car EMI adjustments)
  - Quarterly Rating : Quarterly rating of the driver: 1,2,3,4,5 (higher is better)
  - 
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
  ### 4. Insights & Recommendations:
    - Identify key factors influencing driver attrition
    - Suggest strategies to improve driver retention and optimize hiring
    - Data-driven approach to reducing acquisition costs
