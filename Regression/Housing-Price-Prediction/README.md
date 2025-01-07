# Boston Housing Price Prediction with Decision Trees and Ensemble Methods

This project focuses on predicting housing prices in the Boston area using Decision Tree Regression and various ensemble methods. The dataset used for this project is from the following source:

Dataset source: [Boston Housing dataset](https://www.kaggle.com/datasets/arslanali4343/real-estate-dataset)

---

## Project Overview

The goal of this project is to predict the median value of owner-occupied homes (`MEDV`) in the Boston area. Various models, including Decision Tree Regressor, Random Forest, Bagging Regressor, AdaBoost, Gradient Boosting, and XGBoost, are evaluated and compared to improve predictive accuracy.

---

## Data

The dataset consists of the following features:
- `CRIM`: Per capita crime rate by town.
- `INDUS`: Proportion of non-retail business acres per town.
- `NOX`: Nitric oxide concentration (parts per 10 million).
- `RM`: Average number of rooms per dwelling.
- `AGE`: Proportion of owner-occupied units built before 1940.
- `DIS`: Weighted distances to five Boston employment centers.
- `TAX`: Property tax rate per $10,000.
- `PTRATIO`: Pupil-teacher ratio by town.
- `B`: Proportion of the population that is African-American.
- `LSTAT`: Percentage of lower status of the population.
- `MEDV`: Median value of owner-occupied homes in $1000s (Target Variable).

---

## Results

| Model                        | RMSE       | MSE       | R²       |
|------------------------------|------------|-----------|----------|
| GradientBoostingRegressor     | 2.733306   | 7.470961  | 0.893313 |
| AdaBoostRegressor             | 2.868019   | 8.225531  | 0.882538 |
| Random Forest                 | 3.074958   | 9.455369  | 0.864976 |
| Bagging Regressor            | 3.088889   | 9.541236  | 0.863749 |
| XGBoost                      | 3.397740   | 11.544637 | 0.835141 |
| DecisionTreeRegressor (default) | 3.449101   | 11.896299 | 0.830119 |
| DecisionTreeRegressor with GridSearch | 4.244322 | 18.014272 | 0.742753 |

The results indicate that the Gradient Boosting Regressor achieved the best performance, followed closely by the AdaBoost Regressor.