# Customer Churn Prediction: A Machine Learning Project

## Project Overview

This project predicts customer churn for a telecom company using a comprehensive dataset. By building and evaluating machine learning models, I identified key factors driving customer attrition, providing actionable insights for targeted retention strategies.

## Problem Statement

Customer churn is a significant business challenge. It is more cost-effective to retain existing customers than to acquire new ones. A predictive model helps:

* **Identify high-risk customers:** Enables proactive intervention before service cancellation.
* **Understand churn reasons:** Provides a data-driven diagnosis of why customers are leaving.
* **Develop effective strategies:** Creates personalized retention campaigns based on identified churn drivers.

## Methodology

The project followed a standard data science workflow:

1.  **Data Cleaning:** Handled missing values in `TotalCharges` and converted the column to a numeric data type.
2.  **Exploratory Data Analysis (EDA):** Visualized relationships between features (`tenure`, `MonthlyCharges`, `Contract`) and `Churn`.
3.  **Data Preprocessing:** Transformed raw data by encoding categorical variables and scaling numerical features for model readiness.
4.  **Model Building:** Built and compared a **Logistic Regression** baseline model with a more advanced **Random Forest Classifier**.
5.  **Model Evaluation:** Focused on **recall** and **precision** for the churn class to correctly identify at-risk customers.

**Model Results Summary:**

* **Logistic Regression:** Achieved **79.01%** accuracy, with a churn recall of **52%** and precision of **62%**.
* **Random Forest:** Achieved **79.29%** accuracy, with a churn recall of **48%** and precision of **64%**.

6.  **Feature Importance:** Quantified the influence of each feature to provide actionable business intelligence.

## Key Findings and Recommendations

The models identified several key churn drivers, providing clear, actionable insights:

* **Contract Type:** The most significant finding is that **month-to-month contracts** are the strongest predictor of churn.
* **Customer Lifecycle:** The highest churn rate occurs in the **first few months** of a subscription.
* **Top Feature Drivers:** The model identified the top five features in predicting churn:
    1.  `TotalCharges` (importance: **0.195**)
    2.  `MonthlyCharges` (importance: **0.170**)
    3.  `tenure` (importance: **0.168**)
    4.  `InternetService_Fiber optic` (importance: **0.042**)
    5.  `PaymentMethod_Electronic check` (importance: **0.035**)
* **Service & Cost:** Customers with **higher monthly charges** and **Fiber optic** service are at a higher risk of churning.
* **Payment Method:** Customers using **electronic checks** have a higher churn rate.

Based on these findings, I recommend focusing on incentives for longer-term contracts and implementing proactive outreach for new customers.

## Technologies Used

* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn

## How to Run the Code

1.  Clone this repository: `git clone [repository_url]`
2.  Navigate to the project directory: `cd customer-churn-prediction`
3.  Install the required libraries: `pip install -r requirements.txt`
4.  Open the Jupyter Notebook: `jupyter notebook`

## License

This project is licensed under the MIT License.
```eof# customer-churn-prediction
# customer-churn-prediction
