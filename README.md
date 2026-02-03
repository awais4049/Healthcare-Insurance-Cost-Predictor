# Healthcare Insurance Cost Predictor

A comprehensive machine learning project that predicts healthcare insurance charges based on demographic and health-related features using Linear Regression.

## Overview

This project analyzes healthcare insurance data and builds a predictive model to estimate insurance costs. The implementation includes extensive data preprocessing, feature engineering, model training, and evaluation.

## Features

- **Data Cleaning & Preprocessing**
  - Handling missing values with appropriate imputation strategies
  - Outlier detection and treatment
  - Negative value correction (age, children)
  - String formatting cleanup (charges column)

- **Feature Engineering**
  - Categorical variable encoding (sex, smoker, region)
  - One-hot encoding for multi-class features
  - Binary encoding for boolean features

- **Model Implementation**
  - Linear Regression model
  - Train-validation split approach
  - Comprehensive evaluation metrics

- **Model Evaluation**
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - Mean Absolute Error (MAE)
  - R² Score
  - Feature coefficient analysis

## Dataset Features

The model uses the following features to predict insurance costs:

- **age**: Age of the policyholder
- **sex**: Gender (male/female)
- **bmi**: Body Mass Index
- **children**: Number of dependents
- **smoker**: Smoking status (yes/no)
- **region**: Geographic region (northeast, northwest, southeast, southwest)
- **charges**: Insurance cost (target variable)

## Technologies Used

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **scikit-learn**: Machine learning model and metrics
- **matplotlib/seaborn**: Data visualization (if applicable)

## Project Structure
