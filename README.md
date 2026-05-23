# Explainable AML Detection System

A machine learning system to detect Anti-Money Laundering (AML) patterns in large-scale financial transaction data, with explainability powered by SHAP.

---

## Overview
Money laundering is a critical financial crime that is difficult to detect due to highly imbalanced data and the complexity of laundering patterns. This project builds an explainable ML pipeline using **XGBoost with cost-sensitive learning** to detect suspicious transactions, achieving **96% recall** on a dataset of 45M+ transactions.

SHAP (SHapley Additive exPlanations) is used to provide feature-level explainability, making the model's decisions interpretable for regulatory compliance.

---

## Dataset

**IBM Anti-Money Laundering (AML) Synthetic Transaction Dataset** — available on [Kaggle](https://www.kaggle.com/datasets/ealtman2019/ibm-transactions-for-anti-money-laundering-aml).

### About the Dataset
- Simulates a realistic financial ecosystem involving individuals, companies, and banks
- Covers transaction types: payments, transfers, and purchases
- Models the full money laundering lifecycle: **placement → layering → integration**
- Transactions are labelled as **legitimate** or **laundering**
- Features include: timestamp, sender/receiver accounts, transaction amount, currency, and payment form
- Highly imbalanced: only ~**0.1%** of transactions are laundering (realistic real-world distribution)
- Available in multiple formats (HI/LI) and sizes (small, medium, large)

> An appropriate subset is selected and processed in chronological order to preserve temporal relationships during training and evaluation.

---

## Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Python |
| ML Model | XGBoost (cost-sensitive learning) |
| Explainability | SHAP |
| Data Processing | Pandas, NumPy |
| Evaluation | Scikit-learn |

---

## Key Results

| Metric | Value |
|--------|-------|
| Recall | **96%** |
| Approach | Cost-sensitive XGBoost |
| Explainability | SHAP feature importance |

---
