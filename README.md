# Predictive Customer Analytics

## Overview
This repository contains an end-to-end predictive customer analytics project developed as part of the WiDS (Women in Data Science) program. The project focuses on analyzing customer transaction data to understand purchasing behavior, estimate Customer Lifetime Value (CLV), and predict customer churn.

The work combines conceptual learning with practical implementation and demonstrates how customer behavior data can be translated into actionable business insights.

---

## Project Objectives
- Analyze customer purchasing behavior using transactional data
- Perform RFM (Recency, Frequency, Monetary) based feature engineering
- Estimate Customer Lifetime Value using probabilistic models
- Predict customer churn using supervised machine learning models
- Support strategic marketing and customer retention decisions

---

## Dataset
The project uses the **Online Retail Dataset**, sourced from a publicly available Kaggle mirror of the UCI Machine Learning Repository.

The dataset contains transaction-level data from a UK-based online retailer, including:
- Invoice number
- Customer ID
- Invoice date
- Quantity purchased
- Unit price
- Country

Basic data cleaning steps were applied to remove invalid transactions and prepare the data for analysis.

---

## Repository Structure
predictive-customer-analytics/
├── data/
│ ├── raw/
│ │ └── OnlineRetail.csv
│ └── processed/
│ ├── rfm_features.csv
│ └── clv_results.csv
│
├── notebooks/
│ ├── 03_clv_modeling.ipynb
│ └── 04_churn_prediction.ipynb
│
├── README.md
└── requirements.txt

---

## Feature Engineering and RFM Analysis
Customer behavior is summarized using RFM analysis:
- **Recency**: Time since the customer’s most recent purchase
- **Frequency**: Number of repeat purchases
- **Monetary**: Average transaction value

These features are used as inputs for both CLV modeling and churn prediction.

---

## Customer Lifetime Value (CLV) Modeling
CLV is estimated using probabilistic models implemented through the `lifetimes` library:
- **BG/NBD model** for predicting future purchase frequency
- **Gamma-Gamma model** for estimating average transaction value

CLV is computed over a fixed forecast horizon and used to rank customers based on expected long-term value.

Notebook: `03_clv_modeling.ipynb`

---

## Churn Prediction
Customer churn is modeled as a binary classification problem using RFM-based features.

Models implemented:
- Logistic Regression
- Random Forest Classifier

Model performance is evaluated using precision, recall, F1-score, and confusion matrix analysis.

Notebook: `04_churn_prediction.ipynb`

---

## Key Insights
- Customer value is highly skewed, with a small fraction of customers contributing a large share of revenue
- High-frequency and high-monetary customers exhibit higher predicted CLV
- Random Forest models capture non-linear churn patterns more effectively than linear models
- Combining CLV estimates with churn risk enables better customer prioritization

---

## Learnings
This project provided hands-on experience with:
- Probabilistic customer lifetime modeling
- Feature engineering from transactional data
- Supervised machine learning pipelines
- Model evaluation and interpretation
- Translating analytical results into business recommendations

---

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt

---

## Feature Engineering and RFM Analysis
Customer behavior is summarized using RFM analysis:
- **Recency**: Time since the customer’s most recent purchase
- **Frequency**: Number of repeat purchases
- **Monetary**: Average transaction value

These features are used as inputs for both CLV modeling and churn prediction.

---

## Customer Lifetime Value (CLV) Modeling
CLV is estimated using probabilistic models implemented through the `lifetimes` library:
- **BG/NBD model** for predicting future purchase frequency
- **Gamma-Gamma model** for estimating average transaction value

CLV is computed over a fixed forecast horizon and used to rank customers based on expected long-term value.

Notebook: `03_clv_modeling.ipynb`

---

## Churn Prediction
Customer churn is modeled as a binary classification problem using RFM-based features.

Models implemented:
- Logistic Regression
- Random Forest Classifier

Model performance is evaluated using precision, recall, F1-score, and confusion matrix analysis.

Notebook: `04_churn_prediction.ipynb`

---

## Key Insights
- Customer value is highly skewed, with a small fraction of customers contributing a large share of revenue
- High-frequency and high-monetary customers exhibit higher predicted CLV
- Random Forest models capture non-linear churn patterns more effectively than linear models
- Combining CLV estimates with churn risk enables better customer prioritization

---

## Learnings
This project provided hands-on experience with:
- Probabilistic customer lifetime modeling
- Feature engineering from transactional data
- Supervised machine learning pipelines
- Model evaluation and interpretation
- Translating analytical results into business recommendations

---

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt

---

## Feature Engineering and RFM Analysis
Customer behavior is summarized using RFM analysis:
- **Recency**: Time since the customer’s most recent purchase
- **Frequency**: Number of repeat purchases
- **Monetary**: Average transaction value

These features are used as inputs for both CLV modeling and churn prediction.

---

## Customer Lifetime Value (CLV) Modeling
CLV is estimated using probabilistic models implemented through the `lifetimes` library:
- **BG/NBD model** for predicting future purchase frequency
- **Gamma-Gamma model** for estimating average transaction value

CLV is computed over a fixed forecast horizon and used to rank customers based on expected long-term value.

Notebook: `03_clv_modeling.ipynb`

---

## Churn Prediction
Customer churn is modeled as a binary classification problem using RFM-based features.

Models implemented:
- Logistic Regression
- Random Forest Classifier

Model performance is evaluated using precision, recall, F1-score, and confusion matrix analysis.

Notebook: `04_churn_prediction.ipynb`

---

## Key Insights
- Customer value is highly skewed, with a small fraction of customers contributing a large share of revenue
- High-frequency and high-monetary customers exhibit higher predicted CLV
- Random Forest models capture non-linear churn patterns more effectively than linear models
- Combining CLV estimates with churn risk enables better customer prioritization

---

## Learnings
This project provided hands-on experience with:
- Probabilistic customer lifetime modeling
- Feature engineering from transactional data
- Supervised machine learning pipelines
- Model evaluation and interpretation
- Translating analytical results into business recommendations

---

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
Run the notebooks in the following order:
2.Run the notebooks in the following order:

03_clv_modeling.ipynb

04_churn_prediction.ipynb
Author

Harpreet Singh
Roll Number: 23B2475
Project ID: 100

