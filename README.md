
# House Prices and Doctor Visits Analysis

This project combines two analyses: the first focuses on house prices using the Gamma Generalized Linear Model (GLM), and the second examines the number of doctor visits using data from the 1977–1978 Australian Health Survey. The goal is to explore the relationships between predictor variables and the respective response variables (house prices and doctor visits) in both cases.

## Project Overview

### 1. House Prices Analysis (Gamma GLM)
- **Objective**: Analyze house prices using a Gamma Generalized Linear Model to account for the positive and skewed nature of the response variable (house prices).
- **Key Predictors**: Lot size, number of bedrooms, bathrooms, stories, air conditioning, and other housing features are used to predict house prices.
- **Tech Stack**: Python, Pandas, Scikit-learn, Statsmodels, Matplotlib

### 2. Doctor Visits Analysis (Poisson GLM)
- **Objective**: Model the number of doctor visits based on predictors from the 1977–1978 Australian Health Survey using a Poisson Generalized Linear Model.
- **Key Predictors**: Variables like age, income, chronic conditions, private health insurance, and gender are used to predict the number of doctor visits.
- **Tech Stack**: Python, Pandas, Scikit-learn, Statsmodels, Matplotlib

## Dataset

### 1. House Prices Dataset
The house price data contains 546 observations from Windsor, Canada, for the period of July-September 1987. This dataset includes variables like lot size, bedrooms, bathrooms, and other house-related features.

### 2. Doctor Visits Dataset
The second dataset originates from the 1977–1978 Australian Health Survey, focusing on the number of doctor visits over a two-week period. Variables include age, gender, income, number of chronic conditions, and more.

### Dataset Citations:
- **House Prices Dataset**: [House Prices Dataset](http://qed.econ.queensu.ca/jae/1996-v11.6/anglin-gencay/)
- **Doctor Visits Dataset**: Australian Health Survey (1977–1978)

## File Structure

- **`Doctor Visit analysis - GLM Model.pdf`**: Detailed report discussing the methodology, model performance, and results for both analyses.

## Model and Performance

### 1. House Prices Analysis (Gamma GLM)
- **AIC (Akaike Information Criterion)**: 11951, indicating a good balance between model complexity and performance.
- **Significant Predictors**: Bathrooms, stories, and air conditioning showed a significant relationship with house prices (P-value < 0.05).
- **Residual Deviance**: 24.064 on 534 degrees of freedom, indicating the model explains the data reasonably well.

### 2. Doctor Visits Analysis (Poisson GLM)
- **Chi-Squared P-value**: Both the full and reduced models achieved a p-value of 1, indicating a good fit, though this requires further investigation due to the unusual nature of the value.
- **Significant Predictors**: Age, number of illnesses, and chronic conditions were significant in predicting doctor visits.
- **AIC**: 6735.7 for the full model, indicating a better fit compared to the reduced model.

## Usage

The Jupyter notebook demonstrates the following:
1. **House Prices Analysis**:
    - Loading and preprocessing the house prices dataset.
    - Fitting the Gamma Generalized Linear Model (GLM).
    - Evaluating model performance using metrics such as AIC and residual deviance.
2. **Doctor Visits Analysis**:
    - Loading and preprocessing the doctor visits dataset.
    - Fitting the Poisson Generalized Linear Model (GLM).
    - Evaluating model performance using metrics such as Chi-squared p-value and AIC.


## Acknowledgements

This project was developed as part of an MSc course in Business Analytics.

## License

MIT License
