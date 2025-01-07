# Sentiment Classification on 1,600,000 Tweets

This project focuses on classifying the sentiment of tweets using the **Sentiment140** dataset, which contains 1,600,000 tweets extracted using the Twitter API. The tweets are annotated with sentiment labels (0 = negative, 4 = positive) and can be used for sentiment analysis tasks.

---

## Project Overview

The **Sentiment140** dataset is ideal for performing sentiment analysis, allowing us to predict whether a tweet expresses a positive, neutral, or negative sentiment. It provides a real-world application of machine learning techniques to detect sentiment from raw text data.

---

## Dataset Information

The dataset contains the following fields:

- **target**: The polarity of the tweet (0 = negative, 2 = neutral, 4 = positive).
- **ids**: The unique ID of the tweet (e.g., 2087).
- **date**: The timestamp of the tweet (e.g., Sat May 16 23:58:44 UTC 2009).
- **flag**: The query associated with the tweet. If there is no query, this value is `NO_QUERY`.
- **user**: The username of the person who posted the tweet (e.g., robotickilldozr).
- **text**: The content of the tweet (e.g., "Lyx is cool").

Dataset source: [Sentiment140 Dataset on Kaggle](https://www.kaggle.com/datasets/kazanova/sentiment140)

---

## Results

For this project, the following models were used to classify the sentiment of tweets:

| Model                               | Accuracy | Precision | Recall | F1 Score |
|--------------------------------------|----------|-----------|--------|----------|
| BernoulliNB with CountVectorizer     | 0.769293 | 0.769810  | 0.769293 | 0.769170 |
| BernoulliNB with TfidfVectorizer     | 0.769293 | 0.769810  | 0.769293 | 0.769170 |
| MultinomialNB with CountVectorizer   | 0.768552 | 0.769167  | 0.768552 | 0.768407 |
| MultinomialNB with TfidfVectorizer   | 0.760195 | 0.761246  | 0.760195 | 0.759935 |

