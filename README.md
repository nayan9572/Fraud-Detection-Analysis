# Fraud Detection Analysis:
A Deep Dive into Model Evaluation
This repository contains the code, data, and presentation for an end-to-end machine learning project focused on detecting fraudulent bank transactions. The project goes beyond simple model building to diagnose common challenges like class imbalance and provides a final, strategic recommendation based on a rigorous analytical process.

---

## 🚀 Interactive Report Dashboard (Live Demo)

To make the findings of this project easily accessible and understandable, I have created a single-page interactive web application (`index.html`) that tells the complete story of the analysis.

**Why is this here?** This interactive report is a much more engaging and effective way to present the project's journey than a static notebook. It allows anyone (technical or not) to explore the results and understand the key takeaways.

### **[Click Here to View the Live Interactive Report](https://nayan9572.github.io/Fraud-Detection-Analysis/)**

---
# The Business Problem
Banks and financial institutions face significant financial losses from fraudulent activities. The goal of this project was to develop a machine learning system capable of accurately identifying fraudulent transactions in real-time while minimizing the disruption to legitimate customers. The core technical challenge was a severe class imbalance, with fraudulent transactions making up less than 5% of the total dataset.

# Repository Contents
**index.html:**A single-page web application that serves as the interactive report for this project.
**Fraud Detection analysis assignment.ipynb:** The main Jupyter Notebook containing all the Python code for data analysis, preprocessing, model building, and evaluation.

**Fraud Detection Presentation.pptx:** A slide deck that summarizes the project's journey, key findings, and final recommendation.

**fraud_data.xlsx:** The dataset used for this analysis.


# The Analytical Journey & Key Findings
This project followed a deliberate, iterative process that tells a common story in real-world data science.

**The Accuracy Trap:** Initial models achieved a misleading 95% accuracy but had a Fraud Recall of 0.00, proving they were completely ineffective.

**The SMOTE Breakthrough:** After applying SMOTE to balance the data, a Logistic Regression model successfully achieved a Fraud Recall of 0.60.

**The Limits of Advanced Models:** A critical insight was discovered when advanced models like Random Forest and XGBoost still failed to detect fraud, even on the balanced data.

**A Deeper Diagnosis:** Even after exhaustive hyperparameter tuning, the XGBoost model was unable to reliably detect fraud, leading to the final and most important conclusion.

# Final Recommendation:  It's a Data Problem, Not a Model Problem
The rigorous testing proves that the predictive "signal" from the current features is too weak. The final recommendation is therefore not a model, but a strategy:

## The focus must shift from model tuning to data enhancement and feature engineering.

The most impactful next step is to create more powerful, context-rich features (e.g., avg_amount_vs_user_historical_avg) to provide a stronger signal for a model to learn from.

# How to Run This Project
**1. Clone the repository:**

git clone [https://github.com/nayan9572/Fraud-Detection-Analysis.git](https://github.com/nayan9572/Fraud-Detection-Analysis.git)

**2. Install the required libraries:**
(Note: You will need openpyxl to read .xlsx files with pandas)

pip install pandas scikit-learn matplotlib seaborn imbalanced-learn xgboost jupyter openpyxl
