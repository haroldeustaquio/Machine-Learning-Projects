# Fake Bills Detecter

This project focuses on detecting fake bills using logistic regression analysis. The analysis includes two different approaches to handle missing values: *without Iterative Imputer* and with *Iterative Imputer*. The dataset used for this project is from the following source:

Dataset source: [Fake Bills Dataset](https://www.kaggle.com/datasets/alexandrepetit881234/fake-bills/data)

---

## Project Overview

The goal of this project is to analyze fake bills detection using logistic regression models. We implemented two approaches to handle missing values and evaluated their performance using metrics such as accuracy, F1 score, precision, and recall.

---

## Data

The dataset consists of the following columns:
- `is_genuine`: Boolean indicating whether the bill is genuine.
- `diagonal`: Diagonal measurement of the bill (float).
- `height_left`: Height measurement from the left (float).
- `height_right`: Height measurement from the right (float).
- `margin_low`: Lower margin measurement (float).
- `margin_upper`: Upper margin measurement (float).
- `length`: Length measurement of the bill (float).

---

## Results

| Model                                           | Accuracy   | F1 Score  | Precision | Recall   |
|-------------------------------------------------|------------|-----------|-----------|----------|
| LogisticRegression - newton-cg - balanced       | 0.991803   | 0.993711  | 0.991632  | 0.995798 |
| LogisticRegression - newton-cg - None           | 0.991803   | 0.993737  | 0.987552  | 1.000000 |
| LogisticRegression - newton-cg - balanced       | 0.994667   | 0.995885  | 0.995885  | 0.995885 |
| LogisticRegression - newton-cg - None           | 0.994667   | 0.995885  | 0.995885  | 0.995885 |

Both approaches demonstrated high performance in detecting fake bills, with the logistic regression using *Iterative Imputer* showing slightly better results in terms of accuracy and F1 score.