XGBoost Regressor for Predicting Gym, Pool and Fitness Activities

This project utilizes the XGBoost Regressor to predict various fitness-related activities, including gym access, pool access, classes, squash, and more, based on user data. The model evaluates the importance of different features and provides performance metrics to assess its predictive capabilities.

Introduction

This repository contains Python code that applies the XGBoost Regressor to predict the likelihood of various fitness center activities. The project demonstrates how to preprocess data, train a machine learning model, and visualize feature importance to understand the factors influencing user behavior in a fitness center.

Ensure you have the following libraries installed:

pandas
scikit-learn
matplotlib
seaborn
xgboost

Predict activities for individual members:
The script allows you to input a unique key for a gym member, and it will predict their likely activities based on the trained model.

Project Structure

xgboost_regressor.py: The main Python script that includes data processing, model training, feature importance visualization, and prediction functions.
for_python.xlsx: The dataset used in the project.

Data Processing

The script processes the data by converting date columns into numerical formats, encoding categorical variables, and calculating additional features like the frequency of entry.

Model Training

The XGBoost Regressor is used to train a model for each activity. The script splits the data into training and testing sets, fits the model, and evaluates its performance.

Feature Importance Visualization

The script generates bar plots showing the importance of each feature (e.g., age, gender, membership level) in predicting each activity. These plots help identify which factors are most influential in determining gym or pool access, participation in classes, etc.

Evaluation Metrics

The script calculates and prints several evaluation metrics:

R² (R-squared): Indicates how well the model explains the variance in the data.
MSE (Mean Squared Error): Measures the average squared difference between predicted and actual values.
RMSE (Root Mean Squared Error): The square root of the MSE, providing error measurement in the same units as the target variable.
Prediction for Individual Members

The script includes a function to predict the likelihood of different activities for a specific gym member based on their unique key. It also provides a detailed breakdown of their predicted activities.


