# Code_Alpha-Car-Price-Prediction-With-Machine-Learning

## Project Overview
This project focuses on predicting the selling price of cars based on multiple attributes such as the car's current price, age, kilometers driven, fuel type, transmission, and more. The goal is to build a machine learning model that can predict the selling price of a car based on these features using historical data.

## Objective
The main objective of the project is to:

Predict car selling prices using a machine learning model.

Preprocess data, including handling missing values and encoding categorical variables.

Train a Random Forest Regressor model and evaluate its performance using various metrics.

Visualize results to understand the key factors influencing car pricing.

## Dataset

The dataset contains various features of cars, including:

Selling Price: The price at which the car is sold.

Present Price: The price of the car in the present market.

Driven Kilometers: The total kilometers driven by the car.

Fuel Type: The type of fuel the car uses (e.g., Petrol, Diesel, CNG).

Selling Type: The type of seller (e.g., Dealer, Individual).

Transmission: The transmission type of the car (e.g., Manual, Automatic).

Owner: The number of previous owners of the car.

Car Age: The age of the car (calculated from the year of manufacture).

## Key Columns in the Dataset:

Selling_Price: Target variable (the price to be predicted).

Present_Price: Current market value of the car.

Driven_Kms: The number of kilometers the car has been driven.

Fuel_Type: Type of fuel used in the car (Petrol, Diesel, CNG).

Selling_Type: Type of seller (Dealer or Individual).

Transmission: Type of transmission in the car (Manual or Automatic).

Owner: The number of previous owners.

Car_Age: The age of the car in years.

## Methodology

1. Data Preprocessing

Missing Values: The dataset is checked for missing values, and appropriate handling methods are applied.

Feature Engineering: A new column Car_Age is created by calculating the difference between the current year (2024) and the car's manufacturing year.

Label Encoding: Categorical variables such as Fuel_Type, Selling_Type, and Transmission are encoded into numerical values for the machine learning model to process.

2. Model Selection
   
Random Forest Regressor is used for predicting the car prices due to its ability to handle both linear and non-linear data and its robust performance with a large number of features.

3. Model Evaluation

After training the model, it is evaluated using several metrics to assess its performance:

Mean Absolute Error (MAE): Measures the average magnitude of errors in predictions.

Mean Squared Error (MSE): Indicates how much the predictions deviate from the actual values.

Root Mean Squared Error (RMSE): The square root of MSE, giving the error in the same units as the target variable.

R-squared (R²): Provides the proportion of variance in the target variable explained by the model.

4. Model Deployment
   
Once the model is trained and evaluated, it is saved for future predictions using joblib. This allows the model to be reused on new datasets without retraining.

5. Visualizations
   
Actual vs Predicted Values: A scatter plot is created to compare the actual car prices with the predicted prices.
Feature Importance: A bar chart shows which features are most important in predicting car prices.

## Key Findings

The model achieves an R-squared value of 0.96, meaning that it explains approximately 96% of the variance in the car prices. This indicates that the model performs quite well.

Root Mean Squared Error (RMSE) of 0.97 suggests that the model's predictions are relatively close to the actual values, with a small error margin.

The feature importance plot reveals that features such as Present_Price, Driven_Kms, and Car_Age play a significant role in determining the selling price of cars.

## Model Performance Metrics

Mean Absolute Error (MAE): The model's average error in predicting the price.

Mean Squared Error (MSE): The squared difference between predicted and actual values, used to penalize larger errors.

Root Mean Squared Error (RMSE): A measure that expresses prediction error in the same unit as the target.

R-squared (R²): A statistical measure that shows how well the model explains the variance of the target variable.

## Conclusion

This car price prediction model is highly accurate, as indicated by the high R-squared value and low RMSE. The model can be further improved by using additional features or more sophisticated algorithms. However, it already provides reliable estimates of car prices based on the given dataset.

