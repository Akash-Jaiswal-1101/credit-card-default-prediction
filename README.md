
# Credit Card Default Predictive Framework

## 📌 Project Overview

This project focuses on building a robust predictive framework to forecast credit card defaults for a dataset of **25,000 customers**. The primary goal was to accurately identify high-risk individuals within a minority class (25% default rate) to assist financial institutions in risk mitigation.

By synthesizing domain-specific features and utilizing gradient-boosting algorithms, the framework achieves a balance between predictive power and business interpretability.

## 📊 Key Highlights

* **Target Audience:** 25,000 customers.
* **Class Distribution:** Addressed a 25% minority class imbalance.
* **Model Performance:** Identified **LightGBM** as the optimal classifier.
* **ROC-AUC:** 0.76
* **F1-Score:** 0.46


* **Explainability:** Integrated **SHAP Analysis** to ensure model transparency and actionable business insights.

## 🛠️ Feature Engineering

A significant portion of the performance gain came from synthesizing high-impact features. Key additions include:

* **Delinquency Score:** A synthesized metric designed to capture latent risk in the minority class.
* **Payment Behavior:** Ratios and delays derived from payment history vs. bill amounts.

## 🔬 Model Selection & Evaluation

Comparative analysis was performed across multiple algorithms. LightGBM outperformed others due to its efficiency with categorical features and handling of large data.

| Metric | Score |
| --- | --- |
| **ROC-AUC** | 0.76 |
| **F1-Score** | 0.46 |
| **Recall (Minority Class)** | Optimized for risk detection 
