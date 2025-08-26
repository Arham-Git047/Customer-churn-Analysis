# Customer-churn-Analysis

Customer Churn Prediction Project Report
This repository contains the analysis and a predictive model for customer churn within a telecommunications company. The primary objective of this project is to analyze the key drivers of customer attrition and to develop a robust machine learning model capable of predicting which customers are at risk of churning.

Methodology and Project Workflow
The project was executed through a comprehensive data science pipeline, comprising the following stages:

Data Acquisition and Preliminary Assessment: The initial phase involved loading the Telco customer churn dataset, followed by a preliminary assessment to verify its dimensions, data types, and the presence of missing values.

Data Preprocessing and Feature Engineering: The dataset underwent a series of cleaning and preprocessing steps. This included converting data types, handling missing values, and removing extraneous columns. Furthermore, new features, such as TenureGroup and ServiceCount, were engineered to enhance the predictive power of the models.

Exploratory Data Analysis (EDA): A thorough exploratory data analysis was conducted to understand the underlying data structure. This included the visualization of the target variable distribution, the characteristics of numerical features, and the relationship between various categorical features and churn.

Model Training and Selection: A variety of machine learning classifiers, including Logistic Regression, Random Forest, and XGBoost, were trained. The SMOTE (Synthetic Minority Over-sampling Technique) was applied to the training data to mitigate the effects of class imbalance.

Performance Evaluation: Model performance was rigorously evaluated using standard metrics, including the ROC AUC score, classification reports, and confusion matrices, to ensure a comprehensive assessment of each model's predictive capability.

Feature Importance Analysis: The relative importance of features was analyzed to identify the variables that most significantly influence customer churn.

Summary and Recommendations: The project culminates in a final report that synthesizes key findings and provides data-driven, actionable recommendations for business stakeholders.

System Requirements
The following Python libraries are prerequisites for executing the analysis script:

pandas

numpy

matplotlib

seaborn

scikit-learn

xgboost

imbalanced-learn

These dependencies can be installed via the Python package manager, pip:

pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn

Dataset Information
The analysis utilizes the Telco_Customer_Churn_Dataset.csv. This file must be located in the same directory as the Python script for successful execution.

Operational Instructions
To execute the project script, ensure that all dependencies are installed and the dataset is correctly placed. The script can be run from a command-line interface or an IDE:

python customer_churn_prediction.py

Upon execution, the script will generate a series of performance metrics and display various analytical plots.

Key Findings
The analysis identified several critical factors driving customer churn:

Contract Type: A strong correlation exists between churn and month-to-month contracts, which exhibit a significantly higher churn rate compared to long-term contracts.

Internet Service: Customers with fiber optic internet service demonstrate a higher propensity for churn.

Payment Method: The use of electronic checks as a payment method is associated with an elevated churn probability.

The analysis provides strategic recommendations to address these findings, such as incentivizing long-term contracts and integrating security services into fiber optic packages.

Predictive Model Performance
The XGBoost model was determined to be the most effective classifier for this task, achieving a Receiver Operating Characteristic Area Under the Curve (ROC AUC) of 0.86.
