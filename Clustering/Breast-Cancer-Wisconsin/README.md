# Breast Cancer Wisconsin Diagnostic Clustering using PCA

This project focuses on clustering the Breast Cancer Wisconsin Diagnostic dataset using various algorithms such as K-Means, DBSCAN, and Agglomerative Clustering. We also applied Principal Component Analysis (PCA) to reduce dimensionality for better visualization and clustering performance. The dataset is from the following source:

Dataset source: [Breast Cancer Wisconsin Diagnostic dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)

---

## Project Overview

The goal of this project is to cluster breast cancer diagnostic data and compare different clustering algorithms' performance using evaluation metrics like silhouette score, adjusted Rand index, and V-measure. PCA is used for dimensionality reduction to enhance both clustering efficiency and visualization.

---

## Data

The dataset consists of the following features:
- 30 numeric features related to tumor properties.
- Target variable with two classes: `malignant` and `benign`.
- Includes a total of 569 instances.

---

## Results

| Model                              | Silhouette Score | Davies-Bouldin Score | Adjusted Rand Index | V-Measure | Calinski-Harabasz |
|-------------------------------------|------------------|----------------------|---------------------|-----------|-------------------|
| K-Means - StandardScaler            | 0.34             | 1.50                 | 0.73                | 0.63      | 183.56            |
| K-Means - MinMaxScaler              | 0.43             | 1.11                 | 0.73                | 0.62      | 330.08            |
| DBSCAN - StandardScaler             | 0.36             | 2.14                 | 0.21                | 0.14      | 99.24             |
| DBSCAN - MinMaxScaler               | 0.52             | 1.60                 | 0.05                | 0.04      | 87.77             |
| Agglomerative Clustering - StandardScaler | 0.33         | 1.61                 | 0.66                | 0.54      | 170.39            |
| Agglomerative Clustering - MinMaxScaler | 0.43          | 1.15                 | 0.59                | 0.46      | 317.63            |

K-Means with MinMaxScaler yielded the best performance based on silhouette score and Davies-Bouldin index. However, K-Means with StandardScaler achieved the highest adjusted Rand index and V-Measure, making it the most consistent model overall.
