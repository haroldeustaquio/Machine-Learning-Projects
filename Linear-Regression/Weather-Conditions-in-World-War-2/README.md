# Weather Data During World War II

This project focuses on analyzing weather data collected during World War II. The dataset used for this project is from the following source:

Dataset source: [WeatherWW2 Dataset](https://www.kaggle.com/datasets/smid80/weatherww2/data)

---

## Project Overview

The primary objective of this analysis is to understand weather patterns and explore how they influenced historical events, like military operations, by building machine learning models that predict maximum temperature (`MaxTemp`) based on other weather conditions.

---

## Data

The dataset contains detailed information on weather conditions recorded at various weather stations around the world, including:
- Temperature
- Precipitation
- Snowfall
- Wind speed
- Other weather-related metrics

---

## Results

| model               | r2        | rmse      | mae       |
|---------------------|-----------|-----------|-----------|
| Linear Regression    | 0.986014  | 0.997090  | 0.397755  |
| Lasso                | 0.974618  | 1.343194  | 0.925524  |

Both models are evaluated using various regression metrics, allowing us to compare their performance on the test set.