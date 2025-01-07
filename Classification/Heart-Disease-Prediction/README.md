# Heart Disease Prediction

This project focuses on predicting the risk of heart disease based on various risk factors using logistic regression. The dataset used for this project is from the following source:

Dataset source: [Heart Disease Prediction Dataset](https://www.kaggle.com/datasets/naveengowda16/logistic-regression-heart-disease-prediction)

---

## Project Overview

According to the World Health Organization, an estimated **12 million deaths** occur worldwide every year due to heart diseases. In the United States and other developed countries, cardiovascular diseases account for half of all deaths. Early prognosis of cardiovascular diseases can aid in making decisions regarding lifestyle changes for high-risk patients, ultimately reducing complications.

This research aims to identify the most relevant risk factors for heart disease and predict the overall risk using logistic regression.

---

## Data

The dataset includes various attributes related to individuals' health and lifestyle, which are used to predict the likelihood of heart disease. Key attributes include:

- `male`: Gender of the individual (1 = Male, 0 = Female)
- `age`: Age of the individual.
- `education`: Level of education.
- `currentSmoker`: Indicates if the individual is a current smoker (1 = Yes, 0 = No).
- `cigsPerDay`: Number of cigarettes smoked per day.
- `BPMeds`: Blood pressure medication (1 = Yes, 0 = No).
- `prevalentStroke`: Indicates if the individual has a history of stroke (1 = Yes, 0 = No).
- `prevalentHyp`: Indicates if the individual has hypertension (1 = Yes, 0 = No).
- `diabetes`: Indicates if the individual has diabetes (1 = Yes, 0 = No).
- `totChol`: Total cholesterol level.
- `sysBP`: Systolic blood pressure.
- `diaBP`: Diastolic blood pressure.
- `BMI`: Body Mass Index.
- `heartRate`: Heart rate.
- `glucose`: Glucose level.
- `TenYearCHD`: Indicates if the individual has a risk of coronary heart disease in ten years (1 = Yes, 0 = No).


---

## Results

| Model                                        | Precision | Recall | F1 Score | Support |
|----------------------------------------------|-----------|--------|----------|---------|
| No Heart Disease (0)                         | 0.99      | 0.93   | 0.96     | 1030    |
| Heart Disease (1)                            | 0.24      | 0.77   | 0.37     | 30      |
| **Accuracy**                                 |           |        | 0.93     | 1060    |
| **Macro Average**                            | 0.62      | 0.85   | 0.67     | 1060    |
| **Weighted Average**                         | 0.97      | 0.93   | 0.94     | 1060    |

The best performance was achieved using the `liblinear` solver with `balanced` classes. Importantly, this success was contingent on processing the missing values with the *Iterative Imputer*, which provided a distinct advantage over the other types of imputation methods.