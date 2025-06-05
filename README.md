# Task 6: K-Nearest Neighbors (KNN) Classification - Iris Dataset

## Objective
The aim of this task is to implement the K-Nearest Neighbors (KNN) algorithm on the Iris dataset to perform multi-class classification. The model was trained, evaluated, and visualized to understand the effect of different K values and the importance of feature normalization.

## Dataset
**Iris Dataset**
- Source: [Kaggle - Iris Dataset](https://www.kaggle.com/datasets/uciml/iris)
- Format: CSV (`Iris.csv`)
- Features: SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm
- Target: Species (Iris-setosa, Iris-versicolor, Iris-virginica)

## Tools and Libraries Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Steps Performed

### 1. Data Loading and Cleaning
- Loaded the dataset from CSV
- Dropped the unnecessary `Id` column
- Checked for missing values and data types

### 2. Feature Normalization
- Used `StandardScaler` to normalize features
- Normalization is essential for KNN since it is a distance-based algorithm

### 3. Model Training
- Used `KNeighborsClassifier` from Scikit-learn
- Tried values of K from 1 to 20
- Plotted accuracy vs K to find the optimal value

### 4. Model Evaluation
- Evaluated the model using:
  - Accuracy
  - Confusion matrix
  - Classification report
- Identified best K value based on test accuracy

### 5. Decision Boundary Visualization
- Plotted 2D decision boundaries using only SepalLength and SepalWidth features
- Visualized how the classifier separates classes with the best K

