# Predictive Customer Analytics

Project Status: Completed
Technology: Python, Scikit-Learn, Lifetimes

An end-to-end machine learning project focused on understanding customer purchasing behavior, estimating Customer Lifetime Value (CLV), and predicting churn using transactional data. This project was developed as part of the WiDS (Women in Data Science) program.

## Project Overview
This project demonstrates how raw transaction data can be transformed into actionable business insights using statistical modeling and machine learning.

Key Capabilities:
- Customer segmentation using RFM analysis
- CLV estimation using probabilistic models
- Churn prediction using supervised ML
- Business-driven insights for retention and targeting

## Problem Statement
Businesses often struggle to:
1. Identify high-value customers
2. Predict future revenue contribution
3. Detect customers likely to churn

This project addresses these problems using data-driven techniques.

## Repository Structure
```
predictive-customer-analytics/
├── data/
│   ├── raw/
│   │   └── OnlineRetail.csv
│   └── processed/
│       ├── rfm_features.csv
│       └── clv_results.csv
├── notebooks/
│   ├── 03_clv_modeling.ipynb
│   └── 04_churn_prediction.ipynb
├── requirements.txt
└── README.md
```
## Dataset
Name: Online Retail Dataset
Source: UCI Machine Learning Repository (via Kaggle)
Description: Transaction-level data from a UK-based e-commerce retailer.

Features:
- InvoiceNo, CustomerID, InvoiceDate, Quantity, UnitPrice, Country

Data Cleaning:
- Removed null Customer IDs
- Filtered negative and invalid transactions
- Handled duplicates

## Methodology

1. Feature Engineering (RFM Analysis)
- Recency (R): Days since last purchase
- Frequency (F): Number of purchases
- Monetary (M): Average spend
These features form the foundation for both CLV and churn models.

2. Customer Lifetime Value (CLV)
Implemented using the lifetimes library:
- BG/NBD Model: Predicts purchase frequency
- Gamma-Gamma Model: Estimates average order value

Output: Expected future transactions and predicted revenue per customer.

3. Churn Prediction
Formulated as a binary classification problem.
- Models Used: Logistic Regression, Random Forest Classifier
- Evaluation Metrics: Precision, Recall, F1 Score, Confusion Matrix

## Key Insights
- Revenue is highly concentrated among a small group of customers (Pareto Principle).
- High-frequency customers strongly correlate with high CLV.
- Random Forest outperforms Logistic Regression in capturing churn patterns.
- Combining CLV and churn risk enables smarter customer targeting.

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Lifetimes
- Matplotlib, Seaborn

## How to Run

1. Clone the repository:
git clone https://github.com/your-username/predictive-customer-analytics.git
cd predictive-customer-analytics

2. Install dependencies:
pip install -r requirements.txt

3. Run notebooks:
Execute notebooks/03_clv_modeling.ipynb followed by notebooks/04_churn_prediction.ipynb.

## Future Improvements
- Deploy as a web app (Streamlit or Flask)
- Add customer segmentation dashboard
- Use advanced models (XGBoost, LightGBM)
- Incorporate time-series forecasting

## Author
Harpreet Singh

