# 🏦 Credit Default Prediction

This project predicts the **Probability of Default (PD)** for customers using supervised machine learning techniques. It involves data preprocessing, classification modeling, evaluation, and visualization to help financial institutions assess credit risk effectively.

---

## Problem Statement

Financial institutions face significant risk when customers default on their loans. This project aims to develop a model that can predict whether a customer is likely to default and estimate the associated probability, enabling better credit decisions.

---

## Features

- Data preprocessing and feature engineering  
- Predictive modeling using classification algorithms (e.g., Logistic Regression, Decision Tree, etc.)  
- Probability of Default (PD) calculation  
- Visualization of predicted risk distribution  
- Output DataFrame with:
  - Actual defaults
  - Predicted defaults
  - PD probability
  - Customer status (Default/Not Default)

---

## 🔧 Libraries Used

- `pandas` – Data manipulation and preprocessing  
- `numpy` – Numerical operations  
- `scikit-learn` – Machine learning models and metrics  
- `matplotlib` & `seaborn` – Data visualization  
- `statsmodels` – (Optional) Statistical modeling  

---


- **Class 0 (No Default)**:  
  - 220 correctly predicted  
  - 231 falsely predicted as default

- **Class 1 (Default)**:  
  - 20 correctly predicted  
  - 29 falsely predicted as no default

### 🔹 Classification Report

| Metric       | Class 0 | Class 1 |
|--------------|---------|---------|
| Precision    | 0.88    | 0.08    |
| Recall       | 0.49    | 0.41    |
| F1-Score     | 0.63    | 0.13    |
| Support      | 451     | 49      |

- **Overall Accuracy**: `0.48`  
- **Macro Avg F1-Score**: `0.38`  
- **Weighted Avg F1-Score**: `0.58`  

> 🔍 *Note: The model shows bias towards predicting non-defaults (Class 0), possibly due to class imbalance.*

---

### 🔹 Sample Predictions

| Age | Income       | Loan Amount | Actual | Predicted | PD Probability | Status      |
|-----|--------------|-------------|--------|-----------|----------------|-------------|
| 25  | 27683.14     | 20234.05    | 0      | 1         | 0.5287         | Default     |
| 69  | 29000.98     | 17715.69    | 0      | 1         | 0.5515         | Default     |
| 29  | 23402.27     | 21421.36    | 0      | 1         | 0.5442         | Default     |
| 35  | 28402.92     | 20893.28    | 0      | 1         | 0.5232         | Default     |
| 62  | 40297.00     | 32537.48    | 0      | 0         | 0.3895         | Not Default |
| 52  | 37313.60     | 18972.64    | 0      | 0         | 0.4942         | Not Default |

> 💡 *These examples show predicted probabilities (`PD_Probability`) and final status (`Default` / `Not Default`).*

---

### 📌 Observation

The model is currently overpredicting defaults for customers who did not actually default, suggesting a need for:
- Addressing **class imbalance** (e.g., SMOTE, under-sampling)
- Trying **alternative models** (e.g., XGBoost, Random Forest)
- Adjusting the **decision threshold** (from 0.5 to a better-calibrated value)

---

## 👨‍💻 Author

**Aman**  
📍 Delhi, India  
📧 amankr9481@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/aman-616594130/)  
🐙 [GitHub](https://github.com/aammaann0087)

---

## 📬 Contact

If you have any questions, suggestions, or would like to collaborate on a project, feel free to reach out via [email](mailto:amankr9481@gmail.com) or connect on LinkedIn.

---

## 🙌 Acknowledgements

This project is part of my continuous learning in applied economics, credit risk modeling, and data science.  
Special thanks to:
- Open-source Python community  
- scikit-learn, Seaborn, and Matplotlib developers  
- My mentors and peers who provided feedback on the model and insights




