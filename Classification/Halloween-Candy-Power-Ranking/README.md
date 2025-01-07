# Halloween Candy Power Ranking

This project focuses on ranking Halloween candies based on various attributes, particularly predicting whether a candy contains chocolate. The dataset used for this project is from the following source:

Dataset source: [The Ultimate Halloween Candy Power Ranking](https://www.kaggle.com/datasets/fivethirtyeight/the-ultimate-halloween-candy-power-ranking)

---

## Project Overview

The goal of this project is to analyze and rank Halloween candies using logistic regression to predict chocolate content based on several candy attributes. We evaluated the model's performance using metrics such as precision, F1 score, and recall.

---

## Data

The dataset includes the following attributes for each candy:
- `chocolate`: Does it contain chocolate? (1 = Yes, 0 = No)
- `fruity`: Is it fruit flavored? (1 = Yes, 0 = No)
- `caramel`: Is there caramel in the candy? (1 = Yes, 0 = No)
- `peanutalmondy`: Does it contain peanuts, peanut butter, or almonds? (1 = Yes, 0 = No)
- `nougat`: Does it contain nougat? (1 = Yes, 0 = No)
- `crispedricewafer`: Does it contain crisped rice, wafers, or a cookie component? (1 = Yes, 0 = No)
- `hard`: Is it a hard candy? (1 = Yes, 0 = No)
- `bar`: Is it a candy bar? (1 = Yes, 0 = No)
- `pluribus`: Is it one of many candies in a bag or box? (1 = Yes, 0 = No)
- `sugarpercent`: The percentile of sugar it falls under within the dataset.
- `pricepercent`: The unit price percentile compared to the rest of the set.
- `winpercent`: The overall win percentage according to the 269,000 matchups.

---

## Results

| Model                      | Precision | F1 Score  | Recall   |
|----------------------------|-----------|-----------|----------|
| Logistic Regression         | 1.0       | 0.8421    | 0.7273   |

The model achieved perfect precision while maintaining a reasonable balance between recall and F1 score, indicating high effectiveness in predicting chocolate candies.