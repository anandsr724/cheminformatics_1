# Solubility Prediction Using Machine Learning
This repository demonstrates how machine learning can be applied to predict the solubility of compounds in water based on their molecular descriptors.

## Overview
Solubility is a critical property in various fields, including pharmaceuticals, chemistry, and material science. Predicting solubility based on molecular descriptors allows for faster and more efficient research and development processes.

- In this project:
  -I used machine learning models to predict the solubility of compounds.
  -Feature importance techniques (e.g., Scikit-learn's feature importance, permutation importance, SHAP values) were applied to identify the most significant molecular descriptors.
## Workflow
- Dataset:
The dataset (delaney_mordred_truncated.csv) contains molecular descriptors and measured solubility values for various compounds.
- Preprocessing:
  -Standardized molecular descriptor features using StandardScaler.
  -Split the data into training and test sets for model evaluation.
- Modeling:
  -Trained Linear Regression and Random Forest Regressor models.
  -Evaluated models using metrics such as R² score.
- Feature Importance:
  - Scikit-learn's Feature Importance: Identified important features based on the impurity reduction in the Random Forest model.
  - Permutation Importance: Evaluated the impact of permuting each feature on the model's performance.
SHAP (SHapley Additive exPlanations): Provided detailed insights into feature contributions at both global and instance levels.
- Model Optimization:
  -Selected the top 5 most important features and retrained the models.
  -Compared the performance of models with full features vs. reduced features.
