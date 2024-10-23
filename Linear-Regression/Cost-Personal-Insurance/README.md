# Personal Insurance Cost Prediction

This project focuses on predicting personal insurance costs based on several attributes, including age, gender, BMI, number of children, smoking status, region, and insurance charges. The dataset used for this project is from the following source:

Dataset source: [Personal Insurance Cost Dataset](https://raw.githubusercontent.com/robintux/Datasets4StackOverFlowQuestions/master/CostoPersonalesSeguros.csv)

---

## Project Overview

The goal of this project is to build regression models to predict the insurance charges using different features. We implemented two models: Linear Regression and Lasso Regression, and evaluated their performance using metrics such as RMSE (Root Mean Squared Error), MAPE (Mean Absolute Percentage Error), and R² score.

---

## Data

The dataset consists of the following columns:
- `age`: Age of the individual.
- `sex`: Gender of the individual (male or female).
- `bmi`: Body mass index (BMI).
- `children`: Number of children covered by insurance.
- `smoker`: Whether the individual is a smoker (yes or no).
- `region`: The region where the individual resides (northeast, northwest, southeast, southwest).
- `charges`: Insurance charges billed to the individual.

---

## Models

Two models were implemented in this project:
1. **Linear Regression**
2. **Lasso Regression**

---

## Results

| Model              | RMSE         | MAPE   | R²       |
|--------------------|--------------|--------|----------|
| LinearRegression    | 6006.706131  | 0.430187 | 0.768936 |
| Lasso               | 6006.694553  | 0.430337 | 0.76893  |

Both models performed similarly, with the Linear Regression model achieving slightly better performance in terms of RMSE and MAPE.

---

## Conclusion

The results show that both Linear Regression and Lasso models can predict personal insurance costs with an R² score of approximately 0.77. However, improvements can be made by exploring feature engineering or using more advanced models.

