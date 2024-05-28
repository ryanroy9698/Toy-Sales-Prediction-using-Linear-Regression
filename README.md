# Toy Sales Regression Analysis with Linear and Polynomial Features

In this project, I explored linear regression analysis with additional polynomial features and regularization techniques. Using a toy dataset (LR_data.csv) consisting of 10 features (x1-x10) and a measurement y, I investigated the impact of various regression methods on model performance, which will help predict the number of toys sold as the predictor variable.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Preparation](#data-preparation)
- [Linear Regression](#linear-regression)
- [Linear Regression with Additional Features](#linear-regression-with-additional-features)
- [Linear Regression with Additional Features and Regularization](#linear-regression-with-additional-features-and-regularization)
- [Findings and Results](#findings-and-results)
- [Usage](#usage)

## Project Overview

The project aimed to extend linear regression analysis by incorporating polynomial features and regularization methods. A toy dataset (LR_data.csv) with 10 features (x1-x10) and a measurement y was utilized for experimentation.

## Data Preparation

The dataset was divided into training and validation sets with an 80%:20% split ratio. The data was standardized using StandardScaler from sklearn.

## Linear Regression

Standard linear regression was performed using sklearn.linear_model.LinearRegression. The root mean squared error (RMSE) was calculated for both the training and validation sets.

## Linear Regression with Additional Features

Additional polynomial features up to degree 8 were added to the dataset using sklearn.preprocessing.PolynomialFeatures. Linear regression was then performed on the expanded feature set.

## Linear Regression with Additional Features and Regularization

Ridge regression with regularization was employed using sklearn.linear_model.Ridge. The regularization strength (alpha) was varied from 1E-2 to 1E10 to find the optimal value.

## Findings and Results

- Standard linear regression provided baseline performance.
- Addition of polynomial features improved the model's fit to the data.
- Regularization helped control overfitting, with the choice of alpha influencing model performance.
- The project highlighted the impact of additional features and regularization on linear regression models.

## Usage

### Prerequisites

- Python 3.x
- Scikit-learn
- Numpy
- Matplotlib

### Running the Code

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/regression-analysis.git
    ```
2. Navigate to the project directory:
    ```bash
    cd regression-analysis
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Jupyter Notebook or Python script to perform feature selection, model training, and evaluation:
    ```bash
    jupyter notebook regression_analysis.ipynb```
