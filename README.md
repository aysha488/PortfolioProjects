# Salary Prediction Based on Job Description
# Problem:
The goal of this project is to predict the salary from job description.
# File Guide:
SalaryPredictionDEA.ipynb- This notebook describes obtaining data, EDA and data preprocessing.
SalaryPrediction.ipynb-This notebook contains data preprocessing, modeling, parameter tuning and predictions.
# Basic data description and EDA:
Train dataset has total of 1000000 rows and 8 columns. Six of them are categorical columns() and two are numerical columns. There are no missing and duplicate values in the dataset. 

# Data preprocessing:
There are outliers. We examine the outliers and remove the suspecious outliers. For example, salary less than first quartile clearly indicates they are outliers. Whereas, salaries above third quartile have reasonable ground to be legitimate data because most of them are C level position with higher degree. Finally, categorical data are converted with One hot encoding.

# Baseline Model:
Baseline model is built based on the average salary for industry column and mean squared error(MSE) is calculated 1634.6951926513882 which is very high. 

# Improved Model:
Four ML models are fitted to improve the MSE score and GradientBoosting gives the best result. MSE for gradientBoosting model is 377.45402752571204

# Parameter tuning:
GridSearchCV is used to find the best parameters. Best score for the parameters are found to be … Using best parameters final MSE is found to be…
# Predictions:
Final prediction is made based on the best parameters for the chosen model- gradientBoosting
# Feature Importance:
Feature importance method is used to find the important feature that influences the predictions. Most important features are identified as jobtype, yearsExperience and milefrommetropolices
