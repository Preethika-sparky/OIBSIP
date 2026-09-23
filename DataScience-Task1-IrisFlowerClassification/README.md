# Iris Flower Classification

## Project Overview

This project focuses on classifying Iris flowers into three species using machine learning classification algorithms.

The Iris dataset is loaded directly from `sklearn.datasets.load_iris()` and analyzed using exploratory data analysis and data visualizations.

## Dataset

The Iris dataset contains:

- 150 samples
- 4 numerical features
- 3 target classes

### Features

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

### Target Classes

- Setosa
- Versicolor
- Virginica

## Exploratory Data Analysis

The project includes:

- Dataset shape and data type analysis
- Missing-value check
- Descriptive statistics
- Pairplot visualization
- Box plots for feature distributions
- Feature selection discussion

Petal length and petal width showed clearer separation between the three Iris species compared with the sepal measurements.

## Machine Learning Models

Two classification algorithms were trained:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)

The dataset was divided into training and testing sets using an 80:20 split.

## Model Evaluation

The models were evaluated using:

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-score

### Results

| Model | Accuracy |
|---|---:|
| Logistic Regression | 96.67% |
| KNN | 100% |

KNN achieved the higher accuracy on the test set and correctly classified all 30 test samples.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
DataScience-Task1-IrisFlowerClassification/
│
├── Images/
│
├── Notebooks/
│   └── iris_flower_classification.ipynb
│
└── README.md