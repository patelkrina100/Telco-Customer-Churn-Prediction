# 📊 Telco Customer Churn Prediction

This project analyzes customer churn for a telecommunications company using the **IBM Telco Customer Churn dataset**. The goal is to develop and evaluate machine learning models that predict which customers are likely to leave the service, and to identify the most influential factors contributing to churn.

---

## 📁 Dataset

- **Source**: [Kaggle – Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Context**: This dataset represents customer data from a fictional telecom company, including demographics, service usage, contract information, and churn status.

---

## 🎯 Objectives

- Clean and preprocess the dataset
- Train and evaluate two machine learning models: **Logistic Regression** and **Random Forest**
- Compare model performance using standard metrics
- Identify key features influencing churn
- Visualize model outputs and insights for stakeholders

---

## 🛠️ Tools & Libraries

- **Python**
- **pandas**, **numpy** – Data manipulation
- **scikit-learn** – Modeling and evaluation
- **matplotlib**, **seaborn** – Visualization
- **StandardScaler** – Feature normalization

---

## 🧩 Workflow Summary

1. **Data Cleaning & Preprocessing**
   - Converted `TotalCharges` to numeric
   - Removed `customerID` column and rows with missing values
   - Encoded categorical variables using one-hot encoding
   - Scaled numeric features for logistic regression

2. **Modeling**
   - Split data into training and test sets (80/20 split)
   - Trained both Logistic Regression and Random Forest classifiers
   - Predicted churn outcomes and probability scores

3. **Evaluation**
   - Confusion Matrix
   - Classification Report: Precision, Recall, F1-Score
   - ROC AUC Score
   - ROC Curve Visualization
   - Feature Importance Analysis (Random Forest)

---

## 🔍 Key Results

| Metric                    | Logistic Regression | Random Forest     |
|--------------------------|---------------------|-------------------|
| Accuracy                 | ~80%                | ~79%              |
| ROC AUC Score            | ~0.84               | ~0.82             |
| Precision (Churn = True) | ~0.65               | ~0.63             |
| Recall (Churn = True)    | ~0.57               | ~0.52             |

- **Logistic Regression** slightly outperformed Random Forest in classification metrics and ROC AUC.
- **Random Forest** offered clearer interpretability via feature importances.
- Most influential features: **Contract type**, **Tenure**, **Monthly Charges**, and **Online Security**.

---

## 📌 Conclusions

- Contract-related features were the strongest indicators of churn — especially customers on month-to-month contracts.
- Short tenure and high monthly charges also correlated strongly with churn risk.
- Both models are useful, but Logistic Regression may generalize better for this dataset due to cleaner class separation.

---

## 🚀 Future Improvements

- Perform **hyperparameter tuning** (e.g., GridSearchCV)
- Explore **XGBoost** or **Gradient Boosting**
- Use **SHAP values** for model interpretability
- Build an interactive dashboard using **Streamlit**
- Simulate an **A/B test** for customer retention offers

---

## 👩‍💻 Author

**Krina Patel**  
B.S. Data Science & Business Administration, Northeastern University  
📧 patelkrina100@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/) | [GitHub](https://github.com/) | [Tableau Portfolio](#)
