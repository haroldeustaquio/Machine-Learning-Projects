# Car Price Prediction Project

This project aims to predict car prices based on various features such as manufacturing year, selling price, kilometers driven, fuel type, and engine specifications. By leveraging multiple regression models, this project demonstrates the effectiveness of machine learning techniques in estimating car prices.

- **Dataset Source**: [Car Price Prediction Dataset on Kaggle](https://www.kaggle.com/datasets/sukhmandeepsinghbrar/car-price-prediction-dataset)

---

## Project Overview

The primary objective of this project is to develop predictive models that accurately estimate car selling prices based on given features. To achieve this, we employed several regression models and evaluated their performance using metrics such as R² (coefficient of determination) and RMSE (Root Mean Square Error).

---

## Data

The dataset includes the following features:

| Feature                | Description                                          |
|------------------------|------------------------------------------------------|
| `name`                 | Name of the car model                                |
| `year`                 | Year the car was manufactured                        |
| `selling_price`        | Selling price of the car in the local currency       |
| `km_driven`            | Total kilometers driven by the car                   |
| `fuel`                 | Type of fuel used (e.g., Petrol, Diesel)             |
| `seller_type`          | Type of seller (e.g., Individual, Dealer)            |
| `transmission`         | Transmission type (e.g., Manual, Automatic)          |
| `owner`                | Number of previous owners                            |
| `mileage (km/ltr/kg)`  | Mileage or fuel efficiency of the car                |
| `engine`               | Engine specifications (e.g., 1200 cc)                |

---

## Model Evaluation

The following regression models were implemented and assessed:

| Model                       | R² Score  | RMSE      |
|-----------------------------|-----------|-----------|
| Bagging Regressor           | 0.9586    | 0.0202    |
| Random Forest Regressor     | 0.9585    | 0.0202    |
| XGBoost Regressor           | 0.9509    | 0.0220    |
| Decision Tree Regressor     | 0.9330    | 0.0256    |
| AdaBoost Regressor          | 0.9330    | 0.0256    |
| Gradient Boosting Regressor | 0.9220    | 0.0277    |

The **Bagging Regressor** and **Random Forest Regressor** achieved the highest R² scores, indicating strong predictive performance and low error rates in price estimation. The results demonstrate the effectiveness of ensemble models in capturing complex patterns in the data.

---