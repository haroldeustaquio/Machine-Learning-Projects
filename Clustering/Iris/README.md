# Clustering on the Iris Dataset

This project focuses on the application of different clustering algorithms to the Iris dataset, a classic dataset in machine learning. The goal is to identify natural clusters in the data based on flower characteristics and evaluate the effectiveness of each algorithm using various evaluation metrics. The dataset used for this project is from the following source:

Dataset source: [Iris Dataset](https://archive.ics.uci.edu/ml/datasets/iris)

---

## Project Overview

The goal of this project is to apply and evaluate various clustering algorithms on the Iris dataset to identify natural clusters based on flower characteristics. We implemented three clustering algorithms: KMeans, DBSCAN, and Agglomerative Clustering, and evaluated their performance using metrics such as Silhouette Score, Davies-Bouldin Index, Adjusted Rand Index (ARI), V-Measure, and Calinski-Harabasz Score.

---

## Data

The Iris dataset contains 150 iris flower samples, with the following features:
- `Sepal Length`: Sepal length (cm).
- `Sepal Width`: Sepal width (cm).
- `Petal Length`: Petal length (cm).
- `Petal Width`: Petal width (cm).

The flowers belong to three different species:
- Iris Setosa
- Iris Versicolor
- Iris Virginica

---

## Results

Below are the results of the metrics obtained for each algorithm:

| Model                       | Silhouette | Davies-Bouldin | Adjusted Rand | V-Measure | Calinski-Harabasz |
|-----------------------------|------------|-----------------|----------------|-----------|-------------------|
| **KMeans**                  | 0.504769   | 0.760277        | 0.716342       | 0.741912  | 359.845074        |
| **DBSCAN**                  | 0.523517   | 3.949325        | 0.546422       | 0.664389  | 164.440374        |
| **Agglomerative Clustering** | 0.504800   | 0.747977        | 0.719584       | 0.783740  | 349.254185        |

The KMeans algorithm presents a good separation between clusters, while DBSCAN shows a better Silhouette Score but lower ARI. Agglomerative Clustering shows competitive results to KMeans.

