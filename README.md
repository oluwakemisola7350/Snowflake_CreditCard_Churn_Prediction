# Snowflake_CreditCard_Churn_Prediction
Predicting Stealth churn among active credict card users using Random Forest and XG Boost classifiers, deployed entirely within a Snowflake environment.

## Project Logic & Highlights
* Data Isolation: Filtered the database to analyze the 7,769 active/loyal customers ("CHURN_TARGET = 0") to discover future risks.
* Feature Engineering: Identified and removed target-leaking columns to ensure the models evaluated real customer behavior.
* Model Comparison: Trained and evaluated Random Forest (89% accuracy, 0.90 precision) and XGBoost models.
* The Insight: The pipeline successfully flagged 54 high-risk individuals who have officially stayed with the bank but dropped to "0 ACTIVE_CARDS" identifying a critical "stealth churn" segment.
* Production Deployment: Written the final predictions back to the Snowflake database into a permanent table ("PREDICTED_FUTURE_CHURNERS").
