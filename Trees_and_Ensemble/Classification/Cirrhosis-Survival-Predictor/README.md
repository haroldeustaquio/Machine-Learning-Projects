# Cirrhosis Patient Survival Prediction

This project focuses on predicting the status of cirrhosis patients based on various clinical and demographic features. The dataset used for this project is from the UCI Machine Learning Repository and aims to classify patients' status into three categories: death (D), censored (C), and censored due to liver transplantation (CL). The dataset used for this project is from the following source:

Dataset source: [Cirrhosis Patient Survival Prediction Dataset](https://archive.ics.uci.edu/dataset/878/cirrhosis+patient+survival+prediction+dataset-1)

---

## Project Overview

The goal of this project is to analyze and predict the survival status of cirrhosis patients using various machine learning models. We evaluated the models' performance using metrics such as accuracy, precision, recall, and F1 score.

---

## Data

The dataset includes the following columns:
1. `ID`: Unique identifier for each patient.
2. `N_Days`: Number of days between registration and the earlier of death, transplantation, or study analysis time in July 1986.
3. `Status`: Status of the patient: C (censored), CL (censored due to liver transplant), or D (death).
4. `Drug`: Type of drug administered (D-penicillamine or placebo).
5. `Age`: Age in days.
6. `Sex`: Gender of the patient (M for male, F for female).
7. `Ascites`: Presence of ascites (N for No, Y for Yes).
8. `Hepatomegaly`: Presence of hepatomegaly (N for No, Y for Yes).
9. `Spiders`: Presence of spider angiomata (N for No, Y for Yes).
10. `Edema`: Presence of edema (N for no edema, S for edema without diuretics, Y for edema despite diuretic therapy).
11. `Bilirubin`: Serum bilirubin levels in mg/dl.
12. `Cholesterol`: Serum cholesterol levels in mg/dl.
13. `Albumin`: Albumin levels in gm/dl.
14. `Copper`: Urine copper in µg/day.
15. `Alk_Phos`: Alkaline phosphatase levels in U/liter.
16. `SGOT`: SGOT levels in U/ml.
17. `Triglycerides`: Triglyceride levels in mg/dl.
18. `Platelets`: Platelet count per cubic ml/1000.
19. `Prothrombin`: Prothrombin time in seconds.
20. `Stage`: Histological stage of disease (1, 2, 3, or 4).

---

## Results

Several machine learning models were applied to the dataset, and their performance was evaluated using accuracy, precision, recall, and F1 score. The following models were utilized:

| Model                     | Accuracy | Precision | F1      | Recall   |
|---------------------------|----------|-----------|---------|----------|
| GradientBoostingClassifier | 0.809524 | 0.809524  | 0.739130| 0.680    |
| AdaBoostClassifier        | 0.785714 | 0.794872  | 0.696629| 0.620    |
| CatBoostClassifier        | 0.777778 | 0.843750  | 0.658537| 0.540    |
| BaggingClassifier         | 0.761905 | 0.777778  | 0.651163| 0.560    |
| RandomForestClassifier    | 0.761905 | 0.738095  | 0.673913| 0.620    |
| XGBClassifier             | 0.761905 | 0.738095  | 0.673913| 0.620    |
| DecisionTreeClassifier    | 0.722222 | 0.666667  | 0.631579| 0.600    |

The models demonstrated varying degrees of performance, with the Gradient Boosting Classifier achieving the highest accuracy and precision in predicting patient survival status.