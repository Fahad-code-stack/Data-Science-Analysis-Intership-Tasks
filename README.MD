Iris Classification – Internship Task 1

 Introduction
This task involves building a classification model to predict the species of iris flowers based on their sepal and petal dimensions.

 Dataset Understanding
- Dataset: Iris
- Features: SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm
- Target: Species (Setosa, Versicolor, Virginica)

Data Cleaning & Preparation
- Checked for missing values
- Renamed columns for better readability
- Dropped duplicates (if any)

Exploratory Data Analysis (EDA)
- Histograms and boxplots were used to understand feature distribution
- Pairplot to visualize relationships between variables
- Class distribution checked for balance

Model Training & Testing
- Data was split into training and testing sets
- Classification models used:
  - Logistic Regression
  - Decision Tree Classifier
- Trained and tested models using scikit-learn
Evaluation Metrics
- Accuracy Score
- Confusion Matrix
- Classification Report

Conclusion
- Successfully trained models to classify iris species
- Achieved high accuracy on test data
- Setosa was the most easily classifiable class
