# Customer Churn Prediction

**Customer churn analysis with modular scripts, stakeholder-ready outputs, and reproducible workflows.**

---

## 📌 Project Overview

This project applies the CRISP-DM framework to predict customer churn using behavioral, demographic, and account-level features. It includes:

- Cleaned and imputed customer data
- Exploratory data analysis (EDA) with correlation matrices and PCA
- Clustering for customer segmentation
- Predictive modeling using GLMNET, Random Forest, and XGBoost
- Evaluation with ROC, lift charts, and top-decile targeting
- Stakeholder-ready summaries and visual exports

---

## 🧠 Business Objective

- Identify key drivers of churn
- Segment customers by churn risk and behavior
- Enable targeted retention strategies using predictive lift and gain metrics

---

## 📊 CRISP-DM Workflow

| Step | Description |
|------|-------------|
| 1. Business Understanding | Define churn prediction goals and hypotheses |
| 2. Data Understanding | Load, clean, and explore customer data |
| 3. Data Preparation | Impute missing values, engineer features, remove low-variance predictors |
| 4. Modeling | Train GLMNET, Random Forest, and XGBoost classifiers |
| 5. Evaluation | Compare models using AUC, accuracy, lift, and gain charts |
| 6. Deployment | Export model artifacts and outputs for CRM integration |

---

## 📈 Key Visuals

- **Correlation Matrix of Key Churn Drivers**
- **PCA Biplot with Churn Labels**
- **Cluster Profiles Across Key Metrics**
- **Lift vs. Threshold Optimization**
- **Model Performance Comparison**

All visuals are saved in `outputs/figures/` and ready for stakeholder presentation.

---

## 📂 Project Structure

Customer-Churn/ 
├── data/ # Raw input data 
├── scripts/ # Modular R scripts 
├── outputs/ 
│ ├── figures/ # Visual outputs 
│ └── reports/ # CSV summaries and model comparisons 
├── README.md # Project overview and documentation

---

## 🚀 Deployment Notes

- Models can be saved using `saveRDS()` for scoring new data
- Outputs are CRM-ready and structured for BI dashboard integration
- Suggested next steps: RMarkdown report or Shiny dashboard

---

## 👤 Author

**Bill R. Wathier**  
Graduate Student, Data Analytics  
Southern New Hampshire University  
[LinkedIn](https://www.linkedin.com/in/billwathier) 
[GitHub](https://github.com/bwathier)

---

