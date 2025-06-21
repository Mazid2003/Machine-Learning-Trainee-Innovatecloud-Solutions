# 📅 Day 10:Linear Regression: The Complete Guide

**Date: 20/06/2025**

**🎯 Objective:**

To gain a deep understanding of Linear Regression, one of the most foundational techniques in machine learning, and apply it in both simple and multiple variable scenarios with real-world datasets.

**🧠 Concepts Learned:**

## 🔹 What is Linear Regression?

A statistical method for predicting a continuous target variable using one or more independent variables.

Assumes a linear relationship between features and the outcome.

## 🔹 Types Covered:

Simple Linear Regression: One feature (e.g., Study Hours → Score)

Multiple Linear Regression: Multiple features (e.g., Area, Bedrooms, Age → House Price)

## ✅ Real-World Applications of Linear Regression:

| **Domain**  | **Use Case**                                                                  |
| ----------- | ----------------------------------------------------------------------------- |
| Real Estate | Predict housing prices based on size, location, and other features            |
| Healthcare  | Estimate patient risk score based on age, weight, and vital measurements      |
| Finance     | Predict stock prices and interest rates                                       |
| HR          | Predict employee salary from experience, education, and job role              |
| E-commerce  | Forecast sales based on historical performance and seasonal trends            |
| Education   | Predict student exam scores based on attendance, study hours, and preparation |

## ✳️ 2. Mathematical Formulation

**📌 Simple Linear Regression (Single Feature)**

The equation of a straight line:

**𝑦=𝑚𝑥+𝑐**

In machine learning terms:

**𝑦^=𝛽0+𝛽1𝑥**

Where:

- y^: Predicted Value

- x: Input feature

- 𝛽0: Intercept(bias)

- 𝛽1: coefficient(slope/weight)

🔍 The model learns the optimal values of 𝛽0 and 𝛽1 that minimize prediction error using a cost function like Mean Squared Error (MSE).

**🧮 Multiple Linear Regression (Multiple Features)**

If more than one input feature is involved:

**y^ = β0 + β1x1 + β2x2 +…+ βnxn**

This represents a hyperplane in n-dimensional space.Each 𝛽𝑖 represents the weight or impact of the corresponding feature 𝑥𝑖
on the prediction.

**📘 Interpretation**

Each coefficient (𝛽𝑖) indicates how much the output changes with a one-unit change in that feature, assuming all others are constant.

Linear regression is both predictive and interpretable, making it useful for business forecasting and decision-making.

## 🧪 Hands-On Implementation:

### ✅ Mini Project 1: Student Score Prediction

Dataset: student_scores.csv with features: Hours and target: Score

**Steps Performed:**

Data loading and cleaning

Exploratory Data Analysis (scatter plots, correlation)

Model training using LinearRegression

Evaluation using metrics: MAE, MSE, RMSE, R²

Visualized regression line and residuals

Interpreted impact of each feature

### ✅ Assignment: House Price Prediction

Dataset: housing.csv with features: Area, Bedrooms, Age, etc.

**Steps:**

Selected 3+ features to train a multiple linear regression model

Applied OneHotEncoding to categorical variables

Used Pipeline and ColumnTransformer for cleaner code

Saved the model with joblib for reuse

Evaluated model with R² and residual analysis

**Delivered insights like:**

Each extra bedroom adds ~₹10,000 to house price

Older houses decrease value linearly

## 📊 Metrics Used:

| Metric | Description                                     |
| ------ | ----------------------------------------------- |
| MAE    | Mean of absolute prediction errors              |
| MSE    | Mean of squared errors (penalizes large errors) |
| RMSE   | Root of MSE, easier to interpret                |
| R²     | Explains how well the model fits the data       |

## 📈 Visualizations Created:

Scatter plots of input vs. target

Regression line (actual vs predicted)

Residual plots (to assess bias and model fit)

Correlation heatmaps (for EDA)

## 📁 Deliverables:

✅ student_score_prediction.ipynb

✅ housing_price_prediction.ipynb

✅ Summary PDF (for housing model)

✅ Trained model: housing_price_model.pkl

## ✅ Key Takeaways:

Built and evaluated both simple and multiple linear regression models

Understood when and how to use Linear Regression

Interpreted model coefficients in a business context

Learned best practices for model validation and residual diagnostics
