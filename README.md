# Wine Quality Prediction Using Regression Models

## Project Description

This project analyzes and predicts wine quality using linear regression-based methods. Three regression approaches are implemented and compared:

1. Ordinary Least Squares (OLS) Regression
2. Regularized OLS Regression
3. Stochastic Gradient Descent (SGDRegressor)

The analysis includes data preprocessing, exploratory correlation analysis, predictor selection, model fitting, hyperparameter tuning, model evaluation, and residual diagnostics.

## Dataset

The Wine Quality dataset is publicly hosted on GitHub and is loaded directly into the Python notebook.

Dataset URL:

https://raw.githubusercontent.com/drshikac-sys/wine-quality-regression/refs/heads/main/winequality-red.csv

The response variable is:

- `quality`

The selected predictors used in the regression models are:

- `fixed acidity`
- `volatile acidity`
- `citric acid`
- `alcohol`

## Files

- `Linear_Regression_Analysis_Wine_Quality.ipynb` - Complete Python analysis and model implementation
- `report.pdf` - Final project report
- `README.md` - Project description and instructions

## Requirements

The following Python libraries are required:

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels

## How to Run

1. Download or clone this project repository.
2. Open `Linear_Regression_Analysis_Wine_Quality.ipynb` using Jupyter Notebook, JupyterLab, or Google Colab.
3. Install the required Python libraries if they are not already available.
4. Run the notebook from beginning to end.
5. The dataset will be loaded directly from the public GitHub URL.
6. The notebook performs data preprocessing, exploratory analysis, model training, hyperparameter tuning, evaluation, and visualization.

No local file paths are required to load the dataset.

## Models

### Ordinary Least Squares (OLS)

An OLS regression model is used as the baseline model.

### Regularized OLS

A regularized OLS model is fitted using `statsmodels` with different values of regularization strength and L1 weighting.

### SGD Regression

`SGDRegressor` is used with regularization and hyperparameter tuning. The predictors are standardized before training.

## Evaluation

The models are evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R²

Residual diagnostic plots are also used to examine model assumptions.

## Reproducibility

A fixed random state is used for the train/test split and model configuration where applicable so that the analysis can be reproduced.

The dataset is accessed from the public GitHub URL listed above.
