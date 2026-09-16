# Car Price Prediction with Machine Learning

## Project Overview

This project focuses on predicting the selling price of used cars using machine learning techniques. The project includes exploratory data analysis, data preprocessing, regression model development, model evaluation, and feature importance analysis.

## Objectives

- Analyze the used car dataset and understand important patterns.
- Identify factors that influence car selling prices.
- Preprocess numerical and categorical features for machine learning.
- Build and compare multiple regression models.
- Evaluate models using MAE, RMSE, and R².
- Select the best-performing model for car price prediction.
- Save the final trained model for future predictions.

## Dataset

The project uses a CarDekho vehicle dataset containing 15,411 records and 14 columns.

### Target Variable

- `selling_price`

### Features Used

- `brand`
- `vehicle_age`
- `km_driven`
- `seller_type`
- `fuel_type`
- `transmission_type`
- `mileage`
- `engine`
- `max_power`
- `seats`

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Joblib

## Exploratory Data Analysis

The dataset was analyzed using descriptive statistics and visualizations to understand:

- Distribution of selling prices
- Vehicle age and selling price relationship
- Categorical feature distributions
- Potential outliers and unusual values
- Important patterns within the dataset

## Data Preprocessing

The preprocessing workflow included:

- Checking for missing values
- Checking for duplicate records
- Validating numerical and categorical features
- Separating features and target variable
- Splitting the dataset into training and testing sets
- Standardizing numerical features
- One-hot encoding categorical features

## Machine Learning Models

Two regression models were trained and evaluated:

1. Linear Regression
2. Random Forest Regression

## Model Evaluation

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 182,789 | 396,149 | 0.792 |
| Random Forest | 101,217 | 215,715 | 0.938 |

Random Forest Regression achieved the best overall performance, with lower MAE and RMSE and a higher R² score than Linear Regression.

Therefore, Random Forest was selected as the final model.

## Feature Importance

The Random Forest feature importance analysis showed that:

1. Engine capacity was the most important feature.
2. Kilometers driven was the second most important feature.
3. Vehicle age was the third most important feature.

Several categorical features, including transmission type and specific brands/models, also contributed to the predictions.

Feature importance indicates how much the model relies on a feature for prediction; it does not imply that the feature directly causes the selling price.

## Model Persistence

The trained Random Forest pipeline was saved locally using Joblib as:

`Models/car_price_prediction.pkl`

The model file is excluded from the Git repository because it exceeds GitHub's standard file-size limit.

The notebook can be executed to retrain and recreate the model.

## Project Structure

```text
Car-price-prediction/
│
├── Datasets/
│   └── cardekho_dataset.csv
│
├── Images/
│
├── Models/
│   └── car_price_prediction.pkl
│
├── Notebooks/
│   └── car_price_prediction.ipynb
│
├── .gitignore
├── README.md
└── requirements.txt

How to Run

1. Clone the repository
git clone https://github.com/Preethika-sparky/OIBSIP.git

2. Navigate to the repository
cd OIBSIP

3. Create a virtual environment
python -m venv .venv

4. Activate the environment

For Windows PowerShell:
.\.venv\Scripts\Activate.ps1

5. Install dependencies
pip install -r requirements.txt

6. Open the notebook

Open:

Notebooks/car_price_prediction.ipynb

Run the notebook cells to perform the analysis, train the models, evaluate them, and recreate the model.

Conclusion

This project demonstrates an end-to-end machine learning workflow for used car price prediction, from exploratory data analysis and preprocessing to model training, evaluation, feature importance analysis, and model persistence.

Random Forest Regression provided the best performance among the evaluated models, achieving an R² score of approximately 0.938.