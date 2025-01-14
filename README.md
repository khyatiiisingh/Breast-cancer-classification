# Breast-cancer-classification
Project Overview
This project aims to build and evaluate machine learning models to classify breast cancer data into two categories: malignant and benign. The dataset used in this project is the Breast Cancer Wisconsin dataset, which contains features derived from digital images of breast cancer biopsies.

The objective is to explore different classification algorithms, evaluate their performance, and choose the best model for predicting breast cancer outcomes based on features such as the mean, standard error, and the largest radius of cell nuclei.

Dataset Information
The dataset used in this project is the Breast Cancer Wisconsin dataset (available from UCI Machine Learning Repository). It contains the following:

Number of instances: 569
Number of features: 30
Target classes: Malignant (1) and Benign (0)

Features of the Dataset
Each sample in the dataset corresponds to an image, with features describing characteristics of the cell nuclei extracted from that image. The features are categorized as follows:
Radius: The mean distance from the center to the points on the perimeter.
Texture: Standard deviation of gray-scale intensity values.
Perimeter: Total length around the boundary of the cell nucleus.
Area: Size of the cell nucleus.
Smoothness: Variation in radius lengths (how smooth the boundary is).
Compactness: Calculated as 
Perimeter
2
/
Area
−
1.0
Perimeter 
2
 /Area−1.0 (indicating how compact the nucleus is).
Concavity: The severity of inward curves or concave portions of the boundary.
Concave Points: The number of distinct inward-curving points on the boundary.
Symmetry: Symmetry of the nucleus.
Fractal Dimension: Measure of complexity in the boundary shape, approximated by coastline length minus one.
For each of these features, three variations are provided:

Mean: Average value of the feature.
Standard Error (SE): Measure of variation or deviation for the feature.
Worst: The largest or most severe value (computed as the mean of the three largest values).
This results in a total of 30 features for each sample.

Class Labels
Diagnosis:
M: Malignant (cancerous)
B: Benign (non-cancerous)
This is the target variable for the classification task.
Missing Values:
There are no missing values in this dataset, making preprocessing simpler.

Class Distribution:
Benign (B): 357 samples (63% of the dataset).
Malignant (M): 212 samples (37% of the dataset). This imbalance indicates that benign samples are more common, which may influence model training and evaluation. Proper evaluation metrics like ROC-AUC or precision-recall should be used to handle this imbalance.
Understanding Benign and Malignant

Benign (B):
These tumors are non-cancerous and generally not harmful.
They grow slowly, do not invade surrounding tissues, and do not spread to other parts of the body.
Benign masses are often monitored or surgically removed, but they typically don't pose a significant threat to health.

Malignant (M):
These tumors are cancerous and pose serious health risks.
They grow rapidly, invade nearby tissues, and can spread to other parts of the body through the blood or lymphatic system (a process known as metastasis).
Malignant tumors require aggressive treatment, such as surgery, chemotherapy, or radiation.

Preprocessing Steps:
Data Loading: The dataset is loaded using pandas from a CSV file.
Handling Missing Data: Any missing values (if present) are handled appropriately.
Feature Scaling: Features are scaled using standardization (mean = 0, std = 1) to improve the performance of certain machine learning algorithms.
Data Split: The dataset is split into training and testing sets (80% for training and 20% for testing).
Methodology

The following machine learning algorithms are used in this project:
Logistic Regression: A linear model for binary classification.
Random Forest Classifier: An ensemble method using decision trees to improve prediction accuracy.
These models are trained on the breast cancer dataset and evaluated using performance metrics such as accuracy, precision, recall, and F1 score.

Results
Logistic Regression: Accuracy = 99.12%
Random forest :Accuracy = 96.49%

How to Run the Code
Run the Jupyter Notebook: Open the Jupyter Notebook BREAST CANCER CLASSIFICATION.ipynb:


