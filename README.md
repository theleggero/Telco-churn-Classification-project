------------------------------------------------------------------------
# Telco Customer Churn Prediction Project

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Dataset Description](#dataset-description)
- [Features](#features)
- [Installation and Requirements](#installation-and-requirements)
- [Usage](#usage)
- [Modeling](#modeling)
- [Conclusion](#conclusion)
  

## Overview
The **Telco Customer Churn Prediction Project** is designed to predict customer churn in a telecommunications company. Churn refers to the likelihood of a customer discontinuing their service. By predicting churn, telecom companies can take necessary actions to retain customers, thereby reducing churn rates and increasing profitability.

This project leverages machine learning models to predict whether a customer is likely to churn based on various customer details such as demographics, services subscribed, and usage information.

## Project Structure

```plaintext
telco-churn-prediction/
│
├── data/
│   ├── telco_churn_data.csv       # Dataset file
├── Models/
│   ├── premodel.pkl               # Preprocessing pipeline
│   ├── LogisticRegression.pkl     # Logistic Regression model
│   ├── RandomForest.pkl           # Random Forest model
│   ├── XGBoost.pkl                # XGBoost model
│   ├── KNearest.pkl               # K-Nearest Neighbors model
│   ├── DecisionTree.pkl           # Decision Tree model
├── app.py                         # Streamlit app for customer churn prediction
├── README.md                      # Project documentation
└── requirements.txt               # Required dependencies
```

## Dataset Description
The dataset consists of customer data collected from a telecom company. Each row represents a customer and contains several features related to customer demographics, service subscriptions, billing, and the target label, **Churn**, which indicates whether the customer churned or not.

### Features

| **Column Name**     | **Description** |
|---------------------|-----------------|
| **Gender**           | Whether the customer is male or female. |
| **SeniorCitizen**     | Whether the customer is a senior citizen (1) or not (0). |
| **Partner**           | Whether the customer has a partner (Yes, No). |
| **Dependents**        | Whether the customer has dependents (Yes, No). |
| **Tenure**            | The number of months the customer has stayed with the company. |
| **PhoneService**      | Whether the customer has a phone service (Yes, No). |
| **MultipleLines**     | Whether the customer has multiple phone lines (Yes, No, No phone service). |
| **InternetService**   | Type of internet service (DSL, Fiber optic, No). |
| **OnlineSecurity**    | Whether the customer has online security (Yes, No, No internet service). |
| **OnlineBackup**      | Whether the customer has online backup (Yes, No, No internet service). |
| **DeviceProtection**  | Whether the customer has device protection (Yes, No, No internet service). |
| **TechSupport**       | Whether the customer has tech support (Yes, No, No internet service). |
| **StreamingTV**       | Whether the customer has streaming TV service (Yes, No, No internet service). |
| **StreamingMovies**   | Whether the customer has streaming movie service (Yes, No, No internet service). |
| **Contract**          | The contract term (Month-to-month, One year, Two year). |
| **PaperlessBilling**  | Whether the customer is on paperless billing (Yes, No). |
| **PaymentMethod**     | The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)). |
| **MonthlyCharges**    | The amount charged to the customer on a monthly basis. |
| **TotalCharges**      | The total amount charged to the customer to date. |
| **Churn**             | Whether the customer churned (Yes, No). |

## Installation and Requirements
Before running the app or model scripts, you need to install the required dependencies. Make sure Python (preferably Python 3.7 or later) is installed.

### Install required libraries:
```bash
pip install -r requirements.txt
```

## Usage
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/telco-churn-prediction.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd telco-churn-prediction
   ```
3. **Run the Streamlit app:**
   ```bash
   streamlit run app.py
   ```

4. **Predict churn for individual customers:**
   - In the Streamlit interface, you can input customer data manually to get predictions for a single customer, including their churn likelihood.

5. **Bulk Prediction:**
   - You can upload a CSV file containing multiple customer records to predict churn for all customers in bulk.

## Modeling
This project uses several machine learning models for churn prediction, including:
- **Logistic Regression**: A simple, interpretable model suitable for binary classification problems like churn prediction.
- **Random Forest**: An ensemble model that combines multiple decision trees to improve prediction accuracy.
- **XGBoost**: An optimized gradient boosting algorithm widely used for structured/tabular data.
- **K-Nearest Neighbors (KNN)**: A distance-based algorithm used for classification problems.
- **Decision Tree**: A tree-structured model that predicts the target by learning simple decision rules inferred from the data features.

### Model Training
The models are trained using the preprocessed customer dataset, with **Churn** as the target variable. The preprocessing pipeline handles tasks like encoding categorical variables, handling missing values, and scaling numeric features.

## Conclusion
The Telco Customer Churn Prediction Project helps telecom companies identify customers at risk of churning, enabling proactive retention strategies. By leveraging machine learning models, the app can predict customer churn both individually and in bulk, providing useful insights that can improve customer retention and business profitability.



