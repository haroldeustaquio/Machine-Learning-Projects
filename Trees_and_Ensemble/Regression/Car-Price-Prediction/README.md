# Car Price Prediction Dataset

This project focuses on predicting car prices based on various features such as year of manufacture, selling price, kilometers driven, and engine specifications. The dataset used for this project is from the following source:

Dataset source: [Car Price Prediction Dataset](https://www.kaggle.com/datasets/sukhmandeepsinghbrar/car-price-prediction-dataset)

---

## Project Overview

The goal of this project is to develop predictive models for estimating the selling price of cars using several features. We implemented multiple regression models and evaluated their performance using metrics such as R² and RMSE.

---

## Data

The dataset includes the following features:
| Feature                | Description                                          |
|------------------------|------------------------------------------------------|
| `name`                 | Name of the car                                      |
| `year`                 | The year of manufacture of the car                   |
| `selling_price`        | The selling price of the car in the local currency   |
| `km_driven`            | The total kilometers driven by the car               |
| `fuel`                 | The type of fuel used by the car                     |
| `seller_type`          | The type of seller                                   |
| `transmission`         | The transmission type of the car                     |
| `owner`                | The number of previous owners of the car             |
| `mileage (km/ltr/kg)`  | The mileage or fuel efficiency of the car            |
| `engine`               | The engine specifications of the car                 |

---

## Results

| Model                       | R²        | RMSE      |
|-----------------------------|-----------|-----------|
| BaggingRegressor            | 0.958589  | 0.020162  |
| RandomForestRegressor       | 0.958537  | 0.020175  |
| XGBRegressor                | 0.950877  | 0.021959  |
| DecisionTreeRegressor       | 0.932984  | 0.025649  |
| AdaBoostRegressor           | 0.932984  | 0.025649  |
| GradientBoostingRegressor   | 0.922036  | 0.027665  |