Term Deposit Subscription Prediction (Bank Marketing)

This project predicts whether a client will **subscribe to a term deposit** using the [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing).  
It uses **Logistic Regression** and **Random Forest** for classification, with **explainability** powered by SHAP.


 Project Overview:

Banks often run marketing campaigns to encourage customers to subscribe to term deposits.  
This project builds predictive models to determine the likelihood of subscription, helping in **customer targeting** and **campaign optimization**.

 Key Features:

- Data preprocessing & cleaning  
- One-hot encoding for categorical variables  
- Logistic Regression & Random Forest models  
- Model evaluation with classification reports, confusion matrix, and ROC curves  
- Explainability with **SHAP** (global + local interpretations)  
- All results saved in the `outputs/` folder  


Dataset:

- **File:** `bank-additional-full.csv`  
- **Target variable:** `y` → (`yes` → 1, `no` → 0)  
- **Features:** Demographics, contact info, campaign attributes, and economic indicators  


 Installation:

Clone this repository and install dependencies:

```bash
git clone https://github.com/your-username/bank-term-deposit-prediction.git
cd bank-term-deposit-prediction
pip install -r requirements.txt
```

 Requirements
- Python 3.8+  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- shap  


 Usage:

1. Place the dataset `bank-additional-full.csv` in the project folder.  
2. Open and run the notebook:

```bash
jupyter notebook "Term Deposit Subscription Prediction (Bank Marketing).ipynb"
```

3. All plots and results will be saved inside the **`outputs/`** folder.  



Model Training:

Trained models:

1. **Logistic Regression** (with scaling pipeline)  
2. **Random Forest Classifier**  

Evaluated using:
- Accuracy  
- Precision, Recall, F1-score  
- ROC AUC  


 Outputs:

Generated plots are stored in **`outputs/`**:
- `confusion_matrix.png` → Random Forest confusion matrix  
- `roc_curve.png` → ROC curve  
- `shap_summary.png` → Global feature importance  
- `shap_explain_*.png` → Local explanations for sample predictions  


Explainability:

- **SHAP Summary Plot** → shows most influential features overall  
- **SHAP Force Plot** → explains predictions for individual clients  



Future Improvements:

- Hyperparameter tuning (GridSearchCV / RandomizedSearchCV)  
- Class balancing using SMOTE  
- Web app deployment (Flask/Django/Streamlit)  
- Power BI dashboard integration  



 License:
This project is licensed under the MIT License.  
