# Credit Card Fraud Detection using Machine Learning & Deep Learning

## Project Overview

This project builds an end-to-end fraud detection system for identifying fraudulent credit card transactions using multiple machine learning and anomaly detection techniques.

The dataset is highly imbalanced, making fraud detection a challenging real-world classification problem. Instead of relying only on accuracy, this project evaluates models using precision, recall, F1-score, ROC-AUC, and confusion matrices.

---

## Objectives

* Detect fraudulent transactions with high recall
* Minimize false alarms
* Compare multiple ML approaches
* Apply business-aware threshold optimization
* Interpret important fraud-driving features

---

## Dataset

Public Credit Card Fraud Detection dataset containing anonymized transaction features.

* Total Records: 284,807
* Fraud Cases: 492
* Legitimate Cases: 284,315

---

## Models Implemented

### Supervised Learning

* Logistic Regression
* Random Forest
* XGBoost

### Unsupervised / Deep Learning

* Autoencoder (Anomaly Detection)

---

## Techniques Used

* Train / Validation / Test Split
* StandardScaler
* SMOTE (Class Balancing)
* Threshold Optimization
* ROC Curve Analysis
* Feature Importance

---

## Final Model Comparison

| Model               | Precision | Recall | F1 Score | AUC    |
| ------------------- | --------- | ------ | -------- | ------ |
| Logistic Regression | 0.681     | 0.838  | 0.752    | 0.967  |
| Random Forest       | 0.836     | 0.757  | 0.794    | 0.972  |
| XGBoost             | 0.646     | 0.838  | 0.729    | 0.970  |
| Autoencoder         | 0.843     | 0.797  | 0.819    | Strong |

---

## Key Insights

* Logistic Regression achieved highest recall, useful when missing fraud is costly.
* Random Forest achieved best AUC and low false positives.
* Autoencoder achieved best balance with highest precision and F1-score.
* Model selection should depend on business priorities, not just algorithm popularity.

---

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* TensorFlow / Keras
* Matplotlib
* Seaborn

---

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Open:
`Credit_Card_Fraud_Detection.ipynb`

---

## Future Improvements

* SHAP Explainability
* Hyperparameter Tuning
* Streamlit Deployment
* Real-time Fraud API
* Model Monitoring

---

## Author

Anshul Soni
