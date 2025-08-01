Iris Classification – Internship Task 1
Problem Statement
The goal of this project is to develop a machine learning model that accurately classifies iris flowers into one of three species—Setosa, Versicolor, or Virginica—based on four measurable features: sepal length, sepal width, petal length, and petal width.

This task involves:

Exploring and understanding the classic Iris dataset

Performing exploratory data analysis (EDA) to identify patterns and relationships between features

Training classification models such as Logistic Regression, K-Nearest Neighbors, or Decision Trees

Evaluating the models using accuracy, confusion matrix, and other metrics to determine the most effective classifier.

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
