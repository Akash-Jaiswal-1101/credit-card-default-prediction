
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
| **Recall (Minority Class)** | Optimized for risk detection |

## 💡 Business Insights (SHAP Analysis)

Using SHAP (SHapley Additive exPlanations), we decoded the "black box" model to reveal:

1. **Payment Delays:** The strongest predictor of future default.
2. **Delinquency Score:** Successfully validated as a critical indicator of risk.
3. **Credit Limit vs. Utilization:** Identified non-linear relationships affecting default probability.

## 📁 Repository Structure

```bash
├── data/                   # Dataset (csv files)
├── notebooks/              # Jupyter notebook with EDA & Modeling
├── src/                    # Python scripts for preprocessing
└── README.md               # Project documentation

```

## 🚀 How to Use

1. **Clone the repo:**
```bash
git clone https://github.com/your-username/credit-card-default-prediction.git

```


2. **Install Dependencies:**
```bash
pip install lightgbm shap pandas scikit-learn matplotlib

```


3. **Run the Notebook:**
Open `Akash_Jaiswal_21411003.ipynb` to view the step-by-step analysis and model training.

## 👤 Author

**Akash Jaiswal**



---

### Tips for your GitHub upload:

1. **Notebook Cleanup:** Before uploading, make sure you clear the outputs of the notebook if they contain sensitive data, or keep them if you want to show the graphs directly on GitHub.
2. **Requirements.txt:** Create a `requirements.txt` file containing the libraries used (pandas, numpy, lightgbm, shap, seaborn, matplotlib).
3. **Image:** Use the image I generated for you as the "Social Preview" in your GitHub repository settings to make it look professional!
