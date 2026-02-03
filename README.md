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

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/healthcare-insurance-cost-predictor.git
cd healthcare-insurance-cost-predictor
```

2. Install required packages:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

3. Open the Jupyter notebook:
```bash
jupyter notebook Helathcare_Insurance_Price_Prediction_Complete.ipynb
```

## Usage

1. **Data Loading**: Load the healthcare insurance dataset
2. **Data Preprocessing**: Run preprocessing cells to clean and prepare data
3. **Feature Engineering**: Create encoded features and dummy variables
4. **Model Training**: Train the Linear Regression model on the training set
5. **Evaluation**: Review model performance metrics
6. **Prediction**: Make predictions on validation data

## Key Functions

### `preprocess_dataframe(df)`
Preprocesses the input dataframe by:
- Converting smoker to binary (yes=1, no=0)
- Creating dummy variables for region
- Creating binary variable for sex (is_male)
- Dropping original categorical columns

Returns a fully preprocessed dataframe ready for model training.

## Model Performance

The model provides detailed performance metrics including:
- Training set evaluation
- Validation set predictions
- Feature importance through coefficients
- Comparative analysis between training and validation performance

## Results Interpretation

- **R² Score**: Indicates how well the model explains variance in insurance costs
- **RMSE**: Average prediction error in dollars
- **MAE**: Average absolute prediction error
- **Coefficients**: Show the impact of each feature on insurance cost

Key insights:
- Smoking status typically has the highest impact on insurance costs
- BMI and age are significant predictors
- Regional differences may affect pricing
- Number of children influences cost calculations

## Future Improvements

- [ ] Implement additional regression models (Ridge, Lasso, Random Forest)
- [ ] Feature scaling and normalization
- [ ] Cross-validation for robust evaluation
- [ ] Hyperparameter tuning
- [ ] Feature importance visualization
- [ ] Interactive prediction interface
- [ ] Polynomial features for non-linear relationships
- [ ] Ensemble methods for improved accuracy

## Data Preprocessing Highlights

- **Missing Value Handling**: BMI imputed with mean, children with median
- **Outlier Treatment**: Capped extreme BMI values
- **Data Type Conversion**: Proper numeric and categorical type assignments
- **Consistency Checks**: Standardized region names, smoker values
- **Validation**: Ensured feature alignment between train and validation sets

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Healthcare insurance dataset for model training
- scikit-learn documentation and community
- Machine learning best practices from the data science community

## Disclaimer

This model is for educational and research purposes only. Insurance cost predictions should not be used for actual insurance pricing without proper validation, regulatory compliance, and professional oversight.
