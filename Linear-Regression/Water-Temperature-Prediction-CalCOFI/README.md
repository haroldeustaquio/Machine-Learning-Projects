# Water Temperature Prediction Using Oceanographic Data (CalCOFI Dataset)

This project focuses on predicting water temperature based on various oceanographic measurements. The dataset used for this project is from the following source:

Dataset source: [CalCOFI "bottle" dataset](https://www.kaggle.com/datasets/sohier/calcofi)

---

## Project Overview

The goal of this project is to build regression models to predict the water temperature using different oceanographic features. We implemented two models: Linear Regression and Lasso Regression, and evaluated their performance using metrics such as R² score, RMSE (Root Mean Squared Error), and MAE (Mean Absolute Error).

---

## Data

The dataset consists of the following columns:
- `T_degC`: Water temperature (target variable).
- `Salnty`: Water salinity.
- `O2ml_L`: Oxygen concentration.
- `Depthm`: Water depth.
- `O2Sat`: Oxygen saturation percentage.
- `STheta`: Potential density of the water.
- `more cols`: Additional relevant features.

---

## Results

| model               | r2        | rmse      | mae       |
|---------------------|-----------|-----------|-----------|
| Linear Regression    | 1.000000  | 0.000556  | 0.000109  |
| Lasso                | 0.994442  | 0.315323  | 0.244392  |

The Linear Regression model achieved a high R² score of approximately 1, indicating a near-perfect fit to the data, which is more accurate compared to the Lasso Regression model.
