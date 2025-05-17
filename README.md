This repository contains an interactive Power BI dashboard and a supporting machine learning pipeline for Mortgage Trading Analysis. It is designed to help financial analysts, traders, and portfolio managers gain deeper insights into mortgage-backed securities (MBS) performance, risk metrics, and predictive modeling.

📊 Dashboard Overview
The Power BI dashboard provides a comprehensive overview of mortgage trading activity using simulated or real financial datasets. The report highlights:

Trends and volume in mortgage trading

Spread and interest rate dynamics

Delinquency and loan closure rates

Profitability and ROI KPIs

State-wise and counterparty breakdowns

Drill-down filters for time, region, and loan type

🤖 Machine Learning Extension
As part of the project, we also implemented a machine learning pipeline to predict the property value associated with mortgage loans. The model was trained using clean and structured financial data to enhance insight and automate valuation estimation.

🔧 Features used in the ML model:
Borrower Income (sum_of_income_thousands, monthly_income)

Credit Profile (sum_of_median_fico_score)

Debt Obligations (sum_of_recurring_monthly_debt)

Loan Details (loan_type, loan_purpose, state_code)

🎯 Prediction Target:
sum_of_property_value (Estimated real estate value linked to a loan)

🧠 Model:
Trained using XGBoost Regressor

Achieved an RMSE of ~307,568

Data leakage avoided by excluding derived financial fields such as loan_cost, total_revenue, etc.

📦 Files included:
Cleaned dataset for ML training (final_property_value_dataset.csv)

Trained model and scaler in /models/

Python training script in /notebook/

Requirements for environment setup

✅ Combined Workflow
Use the Power BI dashboard for interactive analysis

Run the ML model to predict property value based on borrower and loan characteristics

Enhance decision-making in mortgage trading, loan packaging, or secondary market analysis

📈 Future Work
Integrate ML model predictions into Power BI via API or Python connector

Expand modeling to include delinquency prediction and loan approval classification

Enhance dashboard with forecasting and anomaly detection modules
