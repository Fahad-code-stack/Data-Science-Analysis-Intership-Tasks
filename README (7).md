Customer Segmentation Using Unsupervised Learning

Project Overview: This project applies **Unsupervised Learning (K-Means
Clustering)** to the **Mall Customers Dataset** in order to segment
customers based on their **annual income** and **spending score**.\
The goal is to identify distinct customer groups and suggest
**data-driven marketing strategies** for each segment.

Dataset: - File: `MallCustomer.csv`\
- Columns: - `CustomerID` -- Unique identifier - `Gender` -- Male /
Female - `Age` -- Customer age - `Annual Income (k$)` -- Annual income
in thousands - `Spending Score (1-100)` -- Shopping behavior score

Steps in the Project:

1.  Import Libraries
    -   pandas, numpy, matplotlib, seaborn, scikit-learn
2.  Data Loading & Validation
    -   File path check added to prevent missing file errors
3.  Exploratory Data Analysis (EDA)
    -   Data summary & distributions\
    -   Gender count plot\
    -   Age distribution\
    -   Spending vs Income scatterplot
4.  Preprocessing
    -   Feature selection (`Annual Income`, `Spending Score`)\
    -   Standardization with `StandardScaler`
5.  Optimal Clusters
    -   Elbow Method (WCSS plot)\
    -   Silhouette Score for validation
6.  K-Means Clustering
    -   Applied KMeans with chosen `k` clusters\
    -   Cluster labels added to dataset
7.  Dimensionality Reduction
    -   PCA applied for 2D visualization of clusters
8.  Cluster Analysis
    -   Cluster summary (mean Age, Income, Spending Score)
9.  Marketing Strategy Suggestions
    -   Tailored strategies for each customer segment

Results: - Clusters formed based on income & spending behavior - PCA
visualization shows well-separated groups\
- Example marketing strategies: - Low income, low spending →
Budget-friendly promotions\
- Low income, high spending → Loyalty rewards\
- High income, low spending → Premium product targeting\
- High income, high spending → VIP/exclusive offers

------------------------------------------------------------------------

How to Run:

1.  Clone this repository or download the project folder.\

2.  Install required dependencies:

    ``` bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

3.  Place `MallCustomer.csv` in the project folder.\

4.  Run the Python script:

    ``` bash
    python customer_segmentation.py
    ```

------------------------------------------------------------------------

Requirements: - Python 3.8+\
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

------------------------------------------------------------------------

Skills Gained: - Unsupervised learning (K-Means Clustering)\
- Dimensionality reduction (PCA)\
- Exploratory Data Analysis (EDA)\
- Strategy development based on cluster insights

------------------------------------------------------------------------

Author: 👤 Fahad Mumtaz\
- 🎓 Data Science & AI - 💼 Project: Customer Segmentation with K-Means
