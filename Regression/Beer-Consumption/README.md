# Beer Consumption Prediction

## Project Description
This project aims to predict beer consumption in liters using weather data and other variables. The dataset used contains daily information about temperature, precipitation, and whether the day was a weekend. Two regression models were applied: **Linear Regression** and **Lasso Regression**. The performance of both models was evaluated based on metrics like RMSE, MAPE, and R². Additionally, scatter plots and residual plots were generated for a better understanding of the predictions.

---

## Data
The dataset used for this project was obtained from the following source:  
[Beer Consumption in São Paulo](https://raw.githubusercontent.com/robintux/Datasets4StackOverFlowQuestions/master/Consumo_cerveza_SP.csv).

The key variables included are:
- **Temperatura Media (C)**: Average daily temperature.
- **Temperatura Minima (C)**: Minimum daily temperature.
- **Temperatura Maxima (C)**: Maximum daily temperature.
- **Precipitacao (mm)**: Precipitation level.
- **Final de Semana**: Whether the day was a weekend (1) or not (0).
- **Consumo de cerveja (litros)**: Daily beer consumption in liters.

---

## Requirements
- pandas
- matplotlib
- seaborn
- scikit-learn

---

## How to Run the Project
1. Install the required libraries.
2. Download the dataset or place the CSV file in the `data` folder.
3. Run the code provided to clean the data, train the models, and evaluate the performance.

---

## Models Used
- **Linear Regression**: A simple linear model for prediction.
- **Lasso Regression**: A regularized model that reduces overfitting.

---

## Results
The performance metrics for both models are as follows:

| Model              | RMSE     | MAPE     | R²       |
|--------------------|----------|----------|----------|
| Linear Regression   | 2.375179 | 0.081708 | 0.700741 |
| Lasso               | 3.146019 | 0.107557 | 0.474977 |

Linear Regression showed better performance compared to Lasso Regression, as reflected by the lower RMSE and higher R² values.