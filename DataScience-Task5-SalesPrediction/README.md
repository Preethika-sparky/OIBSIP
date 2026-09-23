# Sales Prediction Using Python

## OIBSIP Data Science - Task 5

### Project Overview

This project focuses on analyzing the relationship between advertising expenditure and sales and building machine learning models to predict sales.

### Dataset

The project uses the Advertising dataset containing advertising budgets for:

- TV
- Radio
- Newspaper

The target variable is `Sales`.

### Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

### Project Workflow

1. Load and inspect the dataset
2. Check data types and missing values
3. Perform descriptive statistical analysis
4. Perform exploratory data analysis using pairplots
5. Visualize Sales against TV, Radio, and Newspaper advertising
6. Analyze feature correlations using a heatmap
7. Split the data into training and testing sets
8. Train a Linear Regression model
9. Train a Random Forest Regressor
10. Evaluate the models using MAE, RMSE, and R²
11. Analyze residuals of the best-performing model
12. Analyze feature importance

### Model Evaluation

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 1.461 | 1.782 | 0.899 |
| Random Forest Regressor | 0.620 | 0.769 | 0.981 |

The Random Forest Regressor performs better on the test set, with lower MAE and RMSE and a higher R² score.

### Feature Importance

The Random Forest model gives the following feature importance values:

| Advertising Channel | Importance |
|---|---:|
| TV | 0.624810 |
| Radio | 0.362214 |
| Newspaper | 0.012976 |

TV advertising has the highest feature importance in the model, while Newspaper advertising has the lowest.

### Conclusion

The project demonstrates how advertising expenditure can be analyzed and used to predict sales using regression models. Among the evaluated models, Random Forest Regressor provides better test-set performance than Linear Regression. The feature importance analysis indicates that TV advertising is the most influential feature among the three advertising channels in the trained model.

## Project Structure

```text
DataScience-Task5-SalesPrediction/
│
├── Datasets/
│   └── Advertising.csv
│
├── Images/
│
├── Notebooks/
│   └── sales_prediction.ipynb
│
└── README.md