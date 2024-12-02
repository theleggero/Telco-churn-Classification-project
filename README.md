The Telco Churn Classification Project

The objective of the project:
The objective of the Telco Churn Classification project is to forecast customer attrition for a telecom company. This project aims to create a machine learning model capable of accurately identifying customers who might leave, allowing the company to implement proactive measures to retain them. Utilizing customer data such as demographics, account details, service usage, and customer behaviour, the project develops a classification model. The CRIPS-DM framework was adopted. Starting with Business understanding and ending with Model evaluation.


Contents:
1. The objective of the project:
2. Problem Statement
3. Goals:
4. Data Description
5. Exploratory Data Analysis(EDA)
6. Business Questions
7. Machine Learning Model
8. Conclusion
9. How to run the Project



Problem Statement:
Customer attrition presents a significant obstacle for companies in the telecommunications sector, as it is generally more economically viable to keep existing customers than to bring in new ones. In this initiative, we aim to forecast the likelihood of a customer churning by examining a variety of factors. The objective is to analyze customer information to pinpoint essential patterns and trends that indicate when a customer is prone to leaving, thus allowing the business to implement proactive strategies.

Goals
•	Predict: The target variable is the Churn column, which indicates whether the customer has left the company.
•	Explore: Investigate patterns in customer demographics, service usage, and behaviours that contribute to churn.
•	Model: Build and evaluate machine learning models (e.g., logistic regression, decision trees, random forests) to predict churn.

Data Description:
The data in the project contains the following details:

Gender -- Whether the customer is a male or a female
SeniorCitizen -- Whether a customer is a senior citizen or not
Partner -- Whether the customer has a partner or not (Yes, No)
Dependents -- Whether the customer has dependents or not (Yes, No)
Tenure -- Number of months the customer has stayed with the company
Phone Service -- Whether the customer has a phone service or not (Yes, No)
MultipleLines -- Whether the customer has multiple lines or not
InternetService -- Customer's internet service provider (DSL, Fiber Optic, No)
OnlineSecurity -- Whether the customer has online security or not (Yes, No, No Internet)
OnlineBackup -- Whether the customer has online backup or not (Yes, No, No Internet)
DeviceProtection -- Whether the customer has device protection or not (Yes, No, No internet service)
TechSupport -- Whether the customer has tech support or not (Yes, No, No internet)
StreamingTV -- Whether the customer has streaming TV or not (Yes, No, No internet service)
StreamingMovies -- Whether the customer has streaming movies or not (Yes, No, No Internet service)
Contract -- The contract term of the customer (Month-to-Month, One year, Two year)
PaperlessBilling -- Whether the customer has paperless billing or not (Yes, No)
Payment Method -- The customer's payment method (Electronic check, mailed check, Bank transfer(automatic), Credit card(automatic))
MonthlyCharges -- The amount charged to the customer monthly
TotalCharges -- The total amount charged to the customer
Churn -- Whether the customer churned or not (Yes or No)


Exploratory Data Analysis(EDA)

