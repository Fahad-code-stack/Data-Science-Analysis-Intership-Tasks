# Task 2 – Credit Risk Prediction 

 Objective
The goal is to predict whether a loan applicant is likely to **default** or **repay** their loan using classification models.  
We’ll use **Loan Prediction Dataset** from Kaggle.

---

 Steps Performed

 Data Loading
- Imported dataset using **pandas**:  
  ```python
  import pandas as pd
  df = pd.read_csv("Loan Prediction DataSet.csv")
  ```

# Data Understanding
- Checked shape: `df.shape`
- Viewed first rows: `df.head()`
- Checked column names: `df.columns`
- Summarized info: `df.info()`

Data Cleaning
- **Missing values**:
  - Numeric columns → filled with **median**
  - Categorical columns → filled with **mode**
- Removed unnecessary columns if needed

Exploratory Data Analysis (EDA)
- **Loan Status Count** – distribution of approved vs not approved loans
- **Box Plot** – Applicant Income vs Loan Status
- **Histogram** – Loan Amount distribution
- **Count Plot** – Education vs Loan Status

*(Used `matplotlib` & `seaborn` for visualizations)*

 Preprocessing
- **Label Encoding** for categorical features
- **Train-Test Split**: 80% training / 20% testing
- **Scaling**: Applied StandardScaler for Logistic Regression

Model Training
- **Logistic Regression**
- **Decision Tree Classifier**

Model Evaluation
Used:
- `accuracy_score`
- `confusion_matrix`
- `classification_report`

| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | ~78%     |
| Decision Tree       | ~70%     |

---

Insights
- Logistic Regression performed better overall.
- Decision Tree may require tuning to improve accuracy.
- Feature importance can help understand what influences predictions.

---

 How to Run
1. **Clone** this repository or download files
2. Place dataset (`Loan Prediction DataSet.csv`) in the same folder as notebook
3. Install dependencies:
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn
   ```
4. Open Jupyter Notebook:
   ```bash
   jupyter notebook Task2_Credit_Risk_Prediction.ipynb
   ```

---

 Libraries Used
- pandas  
- numpy  
- seaborn  
- matplotlib  
- scikit-learn  

---

 License
This project is under the MIT License.
