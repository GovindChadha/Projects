Project Overview
The Credit Risk Prediction Model is a machine learning-based system designed to assess the likelihood of a loan applicant defaulting on their loan. The model analyzes various financial and demographic factors to predict credit risk, which helps banks, financial institutions, and lenders make better loan approval decisions.

This project covers the entire AI/ML pipeline, including:

Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA)
Feature Engineering
Model Selection & Training (Logistic Regression, Random Forest, XGBoost)
Model Evaluation & Optimization
Deployment as an API
GitHub Integration for Version Control
📊 Data Insights and Findings
1️⃣ Data Cleaning & Preprocessing

The dataset contains financial, demographic, and loan-related features such as loan amount, interest rates, income, credit score, LTV (Loan-to-Value ratio), and more.
We handled missing values by:
Filling numerical columns with median values.
Encoding categorical variables using one-hot encoding.
We normalized numerical features to improve model performance.
2️⃣ Exploratory Data Analysis (EDA)

Loan Default Distribution: The dataset has an imbalance between defaulters and non-defaulters, requiring oversampling (SMOTE) or class weighting.
Key Influencing Factors:
Higher loan amounts increase default risk.
Lower credit scores and higher LTV ratios correlate with defaulting.
Applicants with lower income are more likely to default.
Heatmaps & Correlations showed significant relationships between credit score, income, and default status.
3️⃣ Model Training & Performance

We trained three different models:
Logistic Regression (Baseline Model)
Accuracy: 87.1%
Findings: Works well but struggles with recall for defaulters.
Random Forest (Ensemble Model)
Accuracy: Initially 100% (Overfitting)
Fix: Applied max depth, min sample leaf constraints to prevent overfitting.
XGBoost (Boosting Model)
Accuracy: 99.99% (Overfitting detected)
Fix: Used regularization (L1/L2), subsampling, and learning rate tuning to improve generalization.

🚀 What Can This Model Do?
✅ Automated Credit Risk Assessment:

Helps banks automate loan approvals.
Reduces manual review time by predicting defaults instantly.
✅ Better Decision-Making for Lenders:

Assists banks, financial institutions, and credit agencies in minimizing financial risk.
Helps in setting custom loan interest rates based on applicant risk.
✅ Fraud & Risk Detection:

Can be extended to detect fraudulent loan applications.
Identifies patterns of high-risk applicants.
✅ Future Improvements:

Improve recall for defaulters (handle imbalanced data better).
Test deep learning models (Neural Networks, LSTMs) for better predictions.
Deploy the model as a cloud-based API (AWS, Google Cloud, or Heroku) for real-world use.
Final Thoughts
This project successfully predicts loan defaults and provides an efficient way for financial institutions to assess risk, reduce losses, and automate decision-making. With further hyperparameter tuning and real-world deployment, it can become a powerful AI-driven financial tool. 🚀
