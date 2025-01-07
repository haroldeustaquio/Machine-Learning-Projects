# Weather in Szeged 2006-2016

This project focuses on investigating the relationship between humidity and temperature, and apparent temperature, using weather data from Szeged between 2006 and 2016. The dataset used for this project is from the following source:

Dataset source: [Szeged Weather Dataset](https://www.kaggle.com/datasets/budincsevity/szeged-weather)

---

## Project Overview

The primary objective of this analysis is to determine if there is a significant relationship between humidity, temperature, and apparent temperature, and to predict the apparent temperature based on humidity.

---

## Data

The dataset contains the following columns after cleaning:
- `Formatted Date`: Date of the weather observation.
- `Summary`: Weather summary (e.g., clear, cloudy).
- `Precip Type`: Type of precipitation (e.g., rain, snow).
- `Temperature (C)`: Temperature in Celsius.
- `Apparent Temperature (C)`: Apparent temperature in Celsius.
- `Humidity`: Relative humidity percentage.
- `Wind Speed (km/h)`: Wind speed in kilometers per hour.
- `Wind Bearing (degrees)`: Wind direction in degrees.
- `Visibility (km)`: Visibility distance in kilometers.
- `Pressure (millibars)`: Atmospheric pressure in millibars.

Note: Columns `Loud Cover` and categorical columns were dropped due to lack of variance or non-numeric data.

---

## Results

| model               | r2        | rmse      | mae       |
|---------------------|-----------|-----------|-----------|
| Linear Regression    | 0.990     | 0.951     | 0.743     |
| Lasso                | 0.989     | 0.988     | 0.765     |