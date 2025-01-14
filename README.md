# Breast-cancer-classification
Project Overview
This project aims to build and evaluate machine learning models to classify breast cancer data into two categories: malignant and benign. The dataset used in this project is the Breast Cancer Wisconsin dataset, which contains features derived from digital images of breast cancer biopsies.

The objective is to explore different classification algorithms, evaluate their performance, and choose the best model for predicting breast cancer outcomes based on features such as the mean, standard error, and the largest radius of cell nuclei.

Dataset Information
The dataset used in this project is the Breast Cancer Wisconsin dataset (available from UCI Machine Learning Repository). It contains the following:

Number of instances: 569
Number of features: 30
Target classes: Malignant (1) and Benign (0)
Preprocessing Steps:
Data Loading: The dataset is loaded using pandas from a CSV file.
Handling Missing Data: Any missing values (if present) are handled appropriately.
Feature Scaling: Features are scaled using standardization (mean = 0, std = 1) to improve the performance of certain machine learning algorithms.
Data Split: The dataset is split into training and testing sets (80% for training and 20% for testing).
Methodology
The following machine learning algorithms are used in this project:

Logistic Regression: A linear model for binary classification.
Random Forest Classifier: An ensemble method using decision trees to improve prediction accuracy.
Support Vector Machine (SVM): A classifier that works well in high-dimensional spaces.
K-Nearest Neighbors (KNN): A simple, instance-based learning algorithm that classifies based on proximity to nearest neighbors.
These models are trained on the breast cancer dataset and evaluated using performance metrics such as accuracy, precision, recall, and F1 score.
