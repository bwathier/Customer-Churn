# 📊 Customer Churn Prediction — CRISP-DM Workflow

**Author**: Bill R. Wathier  
**Role**: Graduate Student, Data Analytics  
**Tools**: R, caret, glmnet, randomForest, xgboost, ggplot2, factoextra, pROC  
**Focus**: Predictive modeling, stakeholder-ready reporting, CRM integration

---

## 🔍 Project Summary

This project applies a full-cycle **CRISP-DM analytics workflow** to predict customer churn using behavioral, demographic, and account-level features. The script is modular, reproducible, and designed for stakeholder clarity, with outputs structured for CRM integration and business reporting.

---

## 🧠 Business Objective

- Identify customers most likely to churn and uncover actionable drivers.
- Support retention strategy with interpretable models and top-decile targeting.
- Deliver stakeholder-ready outputs for CRM and dashboard integration.

---

## 🧪 Workflow Overview

### 1. Business Understanding
- Defined hypotheses around usage, tenure, and demographic churn risk.
- Established goals for predictive modeling and stakeholder actionability.

### 2. Data Preparation
- Loaded and cleaned raw churn data.
- Imputed missing values for numeric and categorical features.
- Removed near-zero variance predictors.
- Engineered monthly customer care usage feature.

### 3. Exploratory Analysis & Clustering
- Generated correlation matrices for all numeric features and key churn drivers.
- Performed PCA and visualized scree plot and biplot with churn labels.
- Applied K-means clustering with silhouette and elbow method validation.
- Profiled clusters by churn rate, revenue, usage, and other key metrics.

### 4. Modeling
- Split data into training/testing sets with stratified churn representation.
- Harmonized factor levels across train/test sets.
- Created model matrices and DMatrix structures for reproducibility.
- Trained and evaluated:
  - **GLMNET** (Lasso/Elastic Net)
  - **Random Forest** (caret tuning)
  - **XGBoost** (binary logistic objective)

### 5. Evaluation
- Calculated Accuracy, AUC, and Top-Decile Lift for each model.
- Visualized ROC curves, gain/lift charts, and confusion matrices.
- Optimized classification thresholds based on lift metrics.
- Compared model performance before and after threshold tuning.
- Extracted and visualized variable importance for Random Forest and XGBoost.

### 6. Deployment
- All outputs saved to `outputs/reports/` and `outputs/figures/`.
- Script includes modular preprocessing, error handling, and reproducible structure.
- Future enhancements:
  - Scoring function for new data
  - RMarkdown report or Shiny dashboard
  - CRM export logic for top-decile targeting
  - Python mirror script for cross-platform reproducibility

---

## 📁 Repository Structure

Customer-Churn/ 
├── data/ # Raw input data 
├── outputs/ 
│ ├── reports/ # CSV exports for CRM and stakeholder use 
│ └── figures/ # Visuals for dashboards and presentations 
└── scripts/ # Main R script (CRISP-DM workflow)

---

## 📦 Key Deliverables

- `cluster_summary.csv`: Churn rates and metrics by cluster
- `model_comparison.csv`: Accuracy and AUC across models
- `model_comparison_optimized.csv`: Threshold-tuned performance
- `rf_variable_importance.csv`, `xgb_variable_importance.csv`: Top predictors
- Visuals:
  - PCA plots and biplots
  - Cluster profiles and churn rates
  - ROC overlays and gain/lift charts
  - Confusion matrix heatmaps
  - Variable importance bar plots

---

## 🚀 How to Run

1. Clone this repository.
2. Place raw data in `data/CustomerChurn_Data.csv`.
3. Open `scripts/CustomerChurn_CRISPDM.R` in RStudio.
4. Run the script to generate all outputs.
5. Results will be saved to `outputs/reports/` and `outputs/figures/`.

---

## 📌 Notes

- Designed for reproducibility and public portfolio presentation.
- All visuals and exports are stakeholder-ready.
- Modular structure supports future deployment and dashboard integration.

