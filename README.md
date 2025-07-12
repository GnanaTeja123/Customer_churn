# Customer_churn
📌 Overview
This end-to-end data science project focuses on predicting customer churn in a telecom setting using survival analysis and machine learning techniques. It also offers interpretability using SHAP and Partial Dependence Plots, and culminates in a production-ready Flask app that provides:

Churn probability

SHAP-based customer insights

Survival & hazard curves

Estimated customer lifetime value

🔍 Key Features
📈 Survival Analysis with Kaplan-Meier curves and Cox Proportional Hazard model to estimate customer lifetime

🤖 Random Forest Classifier for churn prediction with optimized hyperparameters using Grid Search CV

🧠 Model Explainability via SHAP, permutation importance, and PDPs

🌐 Deployed Flask Web Application visualizing churn risk, expected lifetime, and actionable insights

🛠️ End-to-end workflow: EDA → Modeling → Explainability → Deployment

📊 Insights from Analysis
Tenure & Loyalty: Longer-tenured customers are significantly less likely to churn.

Contract Type: Month-to-month contracts lead to higher churn, especially with Fiber optic services.

Payment Methods: Electronic check and mailed check users are more prone to churn compared to auto-payment users.

Service Bundling: Customers not subscribed to value-added services (e.g., online security, backup) are more vulnerable.

🤖 Modeling and Performance
Model: Random Forest Classifier with class imbalance handling (class_weight=balanced)

Evaluation:

F1 Score: 0.62

ROC-AUC Score: 0.85

Feature Importance: Key features affecting churn include contract type, tenure, and monthly charges.

🔍 Model Explainability
SHAP: Shows per-customer feature contributions to churn probability

PDPs: Visualize marginal effect of features like tenure, charges, and contract type

Permutation Importance: Robust feature importance rankings

💻 Tech Stack
Languages: Python, HTML/CSS (Flask frontend)

Libraries: scikit-learn, lifelines, pandas, matplotlib, SHAP, Eli5

Deployment: Flask + Heroku

Models:

Random Forest for classification

Cox Proportional Hazard for survival analysis

