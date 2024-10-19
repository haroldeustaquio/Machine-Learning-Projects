# Sentiment Analysis of Airline Tweets

## Dataset Description

This project involves sentiment analysis of tweets related to major U.S. airlines. The data was scraped from Twitter in February 2015, where contributors were asked to classify tweets as positive, negative, or neutral, and further categorize negative reasons (e.g., "late flight," "rude service"). 

The dataset provided on Kaggle includes a reformatted version of the original source, featuring both a CSV file and an SQLite database. The transformation code is available on GitHub.

---

## Dataset Access

You can access the dataset [here](https://www.kaggle.com/code/sathishgsmss/sentiment-airline-dataset).

---

### Dataset Format

The dataset contains the following columns:

- `tweet_id`: Unique identifier for each tweet.
- `airline_sentiment`: Sentiment of the tweet (positive, negative, neutral).
- `airline_sentiment_confidence`: Confidence score for the predicted sentiment.
- `negativereason`: Reason for a negative sentiment.
- `negativereason_confidence`: Confidence score for the negative reason.
- `airline`: Airline associated with the tweet.
- `airline_sentiment_gold`: Gold standard sentiment for comparison.
- `name`: Name of the user who posted the tweet.
- `negativereason_gold`: Gold standard negative reason for comparison.
- `retweet_count`: Number of retweets.
- `text`: Content of the tweet.
- `tweet_coord`: Coordinates of the tweet location (if available).
- `tweet_created`: Timestamp of when the tweet was created.
- `tweet_location`: Location from which the tweet was sent (if available).
- `user_timezone`: Timezone of the user.

---

## Results

The following models were evaluated based on accuracy, precision, recall, and F1 score:

| Model                            | Accuracy | Precision | Recall | F1 Score |
|----------------------------------|----------|-----------|--------|----------|
| Multinomial Balanced CountVect   | 0.7451   | 0.7483    | 0.7451 | 0.7453   |
| Multinomial Balanced Tfidf       | 0.5820   | 0.7323    | 0.5820 | 0.6044   |
| Multinomial CountVect            | 0.7549   | 0.7429    | 0.7549 | 0.7352   |
| Multinomial Tfidf                | 0.6530   | 0.7284    | 0.6530 | 0.5476   |

---

### Key Observations

- The **Multinomial Balanced CountVect** model achieved the highest accuracy and F1 score, indicating its effectiveness in handling the dataset.
- The **Multinomial CountVect** model also performed well but showed lower precision and F1 scores compared to its balanced counterpart.
- The performance of the **Tfidf** models was generally lower, suggesting that Count Vectorization may be more suitable for this dataset.

---

## Conclusion

This sentiment analysis project highlights the challenges and insights from analyzing tweets related to airlines. The balanced CountVect model demonstrates superior performance, underscoring the importance of proper data handling techniques in achieving reliable results in sentiment analysis tasks.
