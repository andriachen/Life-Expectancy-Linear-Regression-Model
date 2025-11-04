# Healthy Life Expectancy Prediction Across Countries

## Overview:
This project predicts healthy life expectancy at the country level using linear and ensemble machine learning methods. The focus is on balancing predictive performance and interpretability. This project was completed individually as part of Break Through Tech AI’s Fall Studio program.

## Models used:
- Linear Regression
- Ridge Regression
- ElasticNet Regression
- Random Forest

## Data:
Country-level aggregated data
- Missing values handled; irrelevant features removed
- Numeric features scaled; missingness indicators added
- Limitation: Only one row per country → small dataset may cause overfitting for complex models.

## Workflow:
1. Data Cleaning: Handling missing values, averaging country-level data, feature removal
2. Feature Engineering: Missingness indicators, scaling numeric features
3. Modeling: Baseline linear regression, Ridge, ElasticNet, Random Forest
4. Evaluation: Cross-validation R² vs Test R², feature importance, outlier handling

## Key Observations:
- Linear models: Generalize better on test data (Test R² ~0.71), interpretable via coefficients
- Random Forest: Higher CV R² (~0.77), captures nonlinear patterns, slight overfitting (Test R² ~0.70)
- ElasticNet: Slightly better CV performance than Ridge, maintains interpretability

## Important Predictors: 
GDP per capita, social support, freedom of choice

## Future Directions:
- Include more years or granular features per country
- Explore feature interactions in linear models
- Apply gradient boosting ensembles for improved prediction
- Visualize feature importance (plots, SHAP values)

## Conclusion
- Ridge & ElasticNet: Robust, interpretable predictions
- Random Forest: Captures nonlinear patterns, minor overfitting due to small dataset
- Model choice depends on interpretability vs predictive flexibility
