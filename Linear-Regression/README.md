# Linear Regression Mini-Projects

This repository contains several mini-projects that apply ``Linear Regression`` and ``Lasso Regression`` models to various datasets. Each project demonstrates the application of regression techniques to solve real-world problems.

---

## Projects

### 1. Beer Consumption Prediction
This project predicts beer consumption in liters based on weather data such as temperature, precipitation, and whether the day is a weekend. We applied ``Linear Regression`` and ``Lasso Regression``, evaluating their performance using metrics like RMSE, MAPE, and R². Visualizations like scatter plots and residual plots help in understanding the model predictions.

Dataset: [Beer Consumption in São Paulo](https://raw.githubusercontent.com/robintux/Datasets4StackOverFlowQuestions/master/Consumo_cerveza_SP.csv)

### 2. Personal Insurance Cost Prediction
Focusing on predicting personal insurance costs, this project utilizes features like age, gender, BMI, number of children, smoking status, and region. Both ``Linear Regression`` and ``Lasso Regression`` models were implemented, and their performances were assessed using RMSE, MAPE, and R² scores. The results show comparable performance, with Linear Regression slightly outperforming Lasso.

Dataset: [Personal Insurance Cost Dataset](https://raw.githubusercontent.com/robintux/Datasets4StackOverFlowQuestions/master/CostoPersonalesSeguros.csv)

### 3. Water Temperature Prediction Using Oceanographic Data (CalCOFI Dataset)
This project aims to predict water temperature using oceanographic measurements. We used ``Linear Regression`` and ``Lasso Regression`` to assess the accuracy of predictions based on salinity, oxygen levels, and depth. The results indicated that Linear Regression performed better than Lasso for this dataset.

Dataset: [CalCOFI "bottle" dataset](https://www.kaggle.com/datasets/sohier/calcofi)

### 4. Weather Data During World War II - Analysis Project
This analysis examines weather data from World War II to understand its impact on historical events. The goal is to predict maximum temperature based on various weather conditions using ``Linear Regression`` and ``Lasso Regression``. The project includes data cleaning, feature selection, and evaluation of model performance.

Dataset: [WeatherWW2 Dataset](https://www.kaggle.com/datasets/smid80/weatherww2/data)

### 5. Weather in Szeged 2006-2016
Investigating the relationship between humidity and apparent temperature, this project predicts apparent temperature using weather data from Szeged. ``Linear Regression`` and ``Lasso Regression`` were applied, with both models showing strong performance, particularly Linear Regression, which achieved an R² score of 0.990.

Dataset: [Szeged Weather Dataset](https://www.kaggle.com/datasets/budincsevity/szeged-weather)

---

## Requirements
- pandas
- matplotlib
- seaborn
- scikit-learn



Feel free to explore each project to understand the methodologies and results in more detail!
