# Car Fuel Efficiency Prediction (Regression Analysis)

This project applies **regression techniques** to predict **miles per gallon (MPG)** using the classic [Auto MPG dataset](https://archive.ics.uci.edu/ml/datasets/auto+mpg).  
The notebook demonstrates a complete data science workflow: from data cleaning and exploratory analysis to building, evaluating, and comparing regression models.

---

##  Project Overview
- **Goal:** Predict car fuel efficiency (MPG) based on vehicle specifications.
- **Dataset:** Auto MPG (398 cars, 9 features, mix of numerical and categorical variables).
- **Approach:** Regression modeling with diagnostics and comparison.

---

## Workflow

1. **Data Cleaning & Preprocessing**
   - Handle missing values in horsepower.
   - Encode categorical features (`cylinders`, `model year`, `origin`).
   - Scale features for fair model comparison.

2. **Exploratory Data Analysis (EDA)**
   - Distributions, scatterplots, and correlations.
   - Pairplots to identify linear relationships.
   - Insight into multicollinearity between predictors.

3. **Modeling**
   - **Baseline model**: Simple linear regression (`mpg ~ weight`).
   - **Multiple regression**: All predictors included.
   - **Polynomial regression**: Capturing nonlinear effects.
   - **Regularization**: Ridge and Lasso to reduce overfitting.

4. **Diagnostics**
   - Residual vs fitted plots.
   - Q-Q plots for normality.
   - Variance Inflation Factor (VIF) for multicollinearity.

5. **Model Comparison**
   - Metrics: R², MSE, RMSE across models.
   - Summary table for performance comparison.

6. **Conclusion**
   - Vehicle weight is the strongest predictor of MPG.
   - Polynomial features slightly improve performance.
   - Lasso regularization helps reduce feature redundancy.
   - Limitations: Small dataset, no external validation.

---

## Repository Contents
- `Polished_Regression_Notebook.ipynb` → Main analysis notebook.
- `README.md` → Project description and usage.
- (Optional) `auto-mpg.csv` → Dataset (if redistribution allowed, otherwise link to source).

---

##  How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/auto-mpg-regression.git
   cd auto-mpg-regression
