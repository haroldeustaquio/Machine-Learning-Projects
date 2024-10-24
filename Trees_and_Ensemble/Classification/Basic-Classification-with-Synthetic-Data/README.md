# Basic Classification with Synthetic Data

This project focuses on implementing decision trees to classify a synthetic dataset. The dataset used for this project is generated using scikit-learn's `make_classification` function.

---

## Project Overview

This mini-project introduces users to the implementation of decision trees, a fundamental algorithm in the field of Machine Learning. By generating and classifying a synthetic dataset, users will learn how to train and evaluate a decision tree model, optimize its hyperparameters, and visualize its internal structure.

---

## Data

The dataset consists of two classes and four features, with the following attributes:
- **Features**: Two informative features and two redundant features.
- **Classes**: Two distinct classes for classification.

This structured environment allows for experimentation with the decision tree model.

---

## Results

| Model                       | Accuracy | Confusion Matrix       |
|-----------------------------|----------|------------------------|
| Decision Tree Classifier (Single Grid) | 0.852    | [120, 8], [29, 93] |
| Decision Tree Classifier (Grid Search) | 0.864    | [119, 9], [25, 97]  |

The model's performance is evaluated using confusion matrices, providing a quantitative measure of its effectiveness. Hyperparameter optimization using `GridSearchCV` resulted in improved accuracy.