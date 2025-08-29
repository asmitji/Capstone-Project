# Capstone Project – E-commerce Price & Discount Prediction

## 📌 Overview
This project builds a machine learning pipeline to predict **discount offers** and **final prices** of products based on e-commerce data.  
It covers the full cycle of data preprocessing, exploratory analysis, feature engineering, and regression modeling.

---

## 📊 Dataset
- **Training Data:** `capstonetrain.csv`
- **Test Data:** `capstone_test.csv`

Key columns include:
- `Rating`, `actprice1`, `price1`
- `noreviews1`, `norating1`
- `star_1f` to `star_5f`
- `fulfilled1`, `platform`, `maincateg`

---

## 🔧 Features of the Pipeline
1. **Data Cleaning & Imputation**
   - Handles missing values with MICE (Iterative Imputer).
   - Fills categorical missing values with gender category (`iswomen`).
   - Removes outliers in `review%`.

2. **Exploratory Data Analysis (EDA)**
   - Heatmaps of missing values.
   - Boxplots & scatterplots for feature distributions.
   - Relationship checks between price, rating, reviews, and offers.

3. **Feature Engineering**
   - Fixes inconsistencies between `actprice1` and `price1`.
   - Creates derived features like `review%`.

4. **Modeling**
   - Models trained:
     - Decision Tree Regressor
     - Random Forest Regressor
     - XGBoost Regressor
   - Evaluation metrics:
     - RMSE (Root Mean Squared Error)
     - R² Score

---

## ⚙️ Installation
Clone this repository and install dependencies:
```bash
git clone <repo_url>
cd capstone-project
pip install -r requirements.txt
