# Task 4: Predicting Insurance Claim Amounts

## Objective
Estimate the medical insurance claim amount based on personal data.

## Dataset
- **Name:** Medical Cost Personal Dataset (synthetic replica generated to be self-contained for this assignment)
- **File:** `insurance.csv`
- **Columns:** `age`, `sex`, `bmi`, `children`, `smoker`, `region`, `charges`

## How to Run
1. Ensure you have Python 3.9+ and the following packages installed:
   - pandas, numpy, scikit-learn, matplotlib, jupyter
2. Open the notebook:
   ```bash
   jupyter notebook task4_insurance.ipynb
   ```
3. Run all cells (Kernel → Restart & Run All).

## What the Notebook Does
- Loads `insurance.csv`
- One-hot encodes categorical features
- Trains a **Linear Regression** model to predict `charges`
- Evaluates performance with **MAE** and **RMSE**
- Visualizes the impact of **age**, **BMI**, and **smoking status** on charges

## Files
- `insurance.csv` — dataset
- `task4_insurance.ipynb` — full notebook
- This `README_Task4.md`

## Notes
- The dataset is synthetically generated to closely mimic realistic patterns (higher costs for smokers, higher BMI/age effects, etc.).
- For better accuracy, try feature engineering and alternative models (e.g., Ridge, Lasso, Gradient Boosting).
