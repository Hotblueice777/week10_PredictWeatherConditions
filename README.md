# Predicting Weather Conditions — Assignment 10

This project builds a machine learning pipeline to **predict next-day maximum temperature (TMAX)** using historical climate data from **San Antonio, Texas**.  
It refines the old version baseline notebook into a **clean, reproducible, and presentation-ready workflow** with improved data quality, feature engineering, and model performance.

---

## Project Overview

| Step                       | Description                                                                           |
| -------------------------- | ------------------------------------------------------------------------------------- |
| **1. Data Cleaning**       | Handled missing and extreme values; applied median imputation and outlier correction. |
| **2. Feature Engineering** | Added lag and rolling-average features; standardized numeric columns.                 |
| **3. Model Training**      | Compared baseline **Linear Regression** with **Random Forest Regressor**.             |
| **4. Model Evaluation**    | Computed MAE, RMSE, and R²; visualized predicted vs actual values and residuals.      |
| **5. Documentation**       | Added clear Markdown explanations and a professional analysis summary.                |

---

## Key Results

| Model                 | MAE     | RMSE   | R²    | Notes                                          |
| --------------------- | ------- | ------ | ----- | ---------------------------------------------- |
| **Linear Regression** | ≈ 0.00  | ≈ 0.00 | 1.000 | Excellent fit, but sensitive to outliers       |
| **Random Forest**     | ≈ 0.009 | ≈ 0.26 | 0.958 | Strong generalization, handles variance better |

> Residual analysis confirmed both models’ errors are centered near zero, with Random Forest showing tighter and more stable residuals.

---

## Insights

- Feature scaling and temporal features improved model stability.
- Random Forest captured nonlinear weather patterns missed by Linear Regression.
- Workflow is modular and easily extendable for additional predictors (e.g., humidity, wind speed).

---

## Tech Stack

- **Language:** Python 3.13
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn
- **Environment:** Jupyter Notebook
- **Version Control:** Git + GitHub

---

## Next Steps

- Add **GridSearchCV** hyperparameter tuning.
- Incorporate **humidity, wind speed, or pressure** variables.
- Deploy the model via **Streamlit** or **Flask** for real-time visualization.

---

### Author

**Joey_Q**  
AI/ML Bootcamp — Assignment 10  
📍 Calgary, Canada
