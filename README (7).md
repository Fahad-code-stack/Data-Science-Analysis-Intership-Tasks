# Loan Default Risk with Business Cost Optimization

## 📌 Objective

The goal of this project is to **predict the likelihood of loan
default** and optimize the **decision threshold** using cost-benefit
analysis.\
This ensures that business decisions (approving or rejecting loans)
minimize financial loss.

## 📊 Dataset

This project uses the **UCI Credit Card Default Dataset**.\
- **Rows:** \~30,000 clients\
- **Columns:**\
- `ID` → Unique client ID (dropped during preprocessing)\
- `LIMIT_BAL` → Amount of credit granted\
- `SEX`, `EDUCATION`, `MARRIAGE`, `AGE` → Demographic features\
- `PAY_0`--`PAY_6` → Past monthly payment delays\
- `BILL_AMT1`--`BILL_AMT6` → Previous bill statements\
- `PAY_AMT1`--`PAY_AMT6` → Previous payments made\
- `default.payment.next.month` → **Target (1 = Default, 0 = No
Default)**

## 🛠 Steps Performed

1.  **Data Preprocessing**
    -   Dropped irrelevant column (`ID`)\
    -   Handled missing values\
    -   One-hot encoded categorical variables\
    -   Scaled numerical features
2.  **Modeling**
    -   Logistic Regression (baseline)\
    -   CatBoost Classifier (if available)
3.  **Evaluation Metrics**
    -   Accuracy, Precision, Recall, F1-Score, ROC-AUC\
    -   Confusion Matrix
4.  **Business Cost Optimization**
    -   Defined costs:
        -   False Positive (rejecting a good client) = 500\
        -   False Negative (accepting a bad client) = 2000\
    -   Adjusted classification threshold to **minimize expected
        business cost**
5.  **Feature Importance**
    -   Top features identified using CatBoost

## 📈 Skills Gained

-   Binary classification modeling\
-   Cost-sensitive evaluation\
-   Risk modeling and credit scoring\
-   Feature importance analysis

## 🚀 How to Run

1.  Clone the repository or download the project files.\

2.  Install dependencies:

    ``` bash
    pip install pandas numpy scikit-learn matplotlib seaborn catboost
    ```

3.  Run the Python script or Jupyter Notebook:

    ``` bash
    python loan_default_cost_optimization.py
    ```

    or

    ``` bash
    jupyter notebook loan_default_cost_optimization.ipynb
    ```

## 📊 Outputs

-   Model performance metrics\
-   Cost vs Threshold optimization curve\
-   Optimal decision threshold\
-   Feature importance visualization (CatBoost)

## 📂 Project Structure

    ├── Loan_Default_Cost_Optimization.py   # Full training & evaluation script
    ├── README.md                           # Project documentation
    ├── UCI_Credit_Card.csv                 # Dataset (place here)

------------------------------------------------------------------------

👨‍💻 **Author:** Fanoltas\
📌 AI & Data Science Enthusiast \| Data Analyst in progress
