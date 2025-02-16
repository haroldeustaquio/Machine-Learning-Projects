# Beer Consumption Prediction

## Overview

This project aims to predict beer consumption in liters using weather data and other variables. The dataset contains daily information about temperature, precipitation, and whether the day was a weekend. By analyzing these factors, we can gain insights into the patterns and trends that influence beer consumption.

**Content**

- [Data Description](#data-description)
- [Requirements](#requirements)
- [Conclusion](#conclusion)

---

## Data Description
The dataset used for this project was obtained from the following source: [Beer Consumption in São Paulo](https://raw.githubusercontent.com/robintux/Datasets4StackOverFlowQuestions/master/Consumo_cerveza_SP.csv).

The key variables included are:
- **Temperatura Media (C)**: Average daily temperature.
- **Temperatura Minima (C)**: Minimum daily temperature.
- **Temperatura Maxima (C)**: Maximum daily temperature.
- **Precipitacao (mm)**: Precipitation level.
- **Final de Semana**: Whether the day was a weekend (1) or not (0).
- **Consumo de cerveja (litros)**: Daily beer consumption in liters.

---

## Requirements

```bash
pip install numpy pandas scikit-learn matplotlib scipy 
```

---

## Conclusion

- **Best realistic option:** **Gradient Boosting Pro or AdaBoost Pro**.
- **Gradient Boosting Pro** is a powerful option with tuned hyperparameters.
- **AdaBoost Pro** is more stable and less prone to overfitting.
