# Predicting MBTI Personality Types

This project aims to predict the Myers-Briggs Type Indicator (MBTI) personality types using a synthetic dataset from Kaggle. The dataset includes over 100,000 samples and contains demographic information, interest areas, and personality scores that help determine an individual's MBTI type.

Dataset source: [Predict People Personality Types Dataset](https://www.kaggle.com/datasets/stealthtechnologies/predict-people-personality-types)

---

## Project Overview

This synthetic dataset is designed to explore and predict MBTI personality types based on a combination of demographic factors, interest areas, and personality scores.

---

## Data

The dataset includes the following features:

- **Age**: A continuous variable representing the age of the individual.
- **Gender**: A categorical variable indicating the gender of the individual ('Male' or 'Female').
- **Education**: A binary variable where a value of 1 indicates the individual has at least a graduate-level education (or higher), and 0 indicates an undergraduate, high school level, or uneducated.
- **Interest**: A categorical variable representing the individual's primary area of interest.
- **Introversion Score**: A continuous variable (0-10) representing the individual's tendency toward introversion versus extraversion (higher scores indicate a greater tendency toward extraversion).
- **Sensing Score**: A continuous variable (0-10) representing the individual's preference for sensing versus intuition (higher scores indicate a preference for sensing).
- **Thinking Score**: A continuous variable (0-10) indicating the individual's preference for thinking versus feeling (higher scores indicate a preference for thinking).
- **Judging Score**: A continuous variable (0-10) representing the individual's preference for judging versus perceiving (higher scores indicate a greater preference for judging).
- **Personality**: The target variable containing the MBTI personality type.

---

## Results

| Model                                     | Accuracy | F1 Score | Precision | Recall   |
|-------------------------------------------|----------|----------|-----------|----------|
| Logistic Regression - newton-cg - None    | 0.826076 | 0.822679 | 0.821617  | 0.826076 |
| Logistic Regression - newton-cg - balanced | 0.764518 | 0.778458 | 0.815118  | 0.764518 |
| Logistic Regression - sag - None          | 0.172597 | 0.168800 | 0.165290  | 0.172597 |
| Logistic Regression - sag - balanced      | 0.117364 | 0.122100 | 0.160197  | 0.117364 |
| Logistic Regression - saga - None         | 0.175044 | 0.170186 | 0.165811  | 0.175044 |
| Logistic Regression - saga - balanced     | 0.135974 | 0.148503 | 0.166727  | 0.135974 |
| Logistic Regression - lbfgs - None        | 0.187303 | 0.175951 | 0.167419  | 0.187303 |
| Logistic Regression - lbfgs - balanced    | 0.112054 | 0.131062 | 0.165167  | 0.112054 |
