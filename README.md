# RCA CIE 2 – Activity 2: Binary Classification using Logistic Regression

## 1. Project Overview

This project is submitted for Regression and Classification Algorithms (RCA), CIE 2 – Activity 2: Binary Classification Activity.

The objective is to build and evaluate a Logistic Regression model that predicts whether a customer recommends a women's clothing product based on information recorded in the review.

**Role:** Data Scientist analysing customer review recommendations.

## 2. Dataset Information

- **Dataset Name:** Women's E-Commerce Clothing Reviews
- **Dataset Source:** Kaggle
- **Dataset Link:** https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews
- **Dataset Size:** 23,486 rows and 11 columns.

### Selected Features

**Input Features (X):**
- Age
- Rating
- Positive Feedback Count

**Target Variable (y):**
- Recommended IND

Target classes:
- 0 – Not Recommended
- 1 – Recommended

Each row represents one customer review.

## 3. Work Completed

The following tasks have been performed in the Jupyter Notebook:

1. Importing required Python libraries.
2. Loading and understanding the dataset.
3. Data inspection and exploratory data analysis.
4. Checking missing values and duplicate records.
5. Data cleaning and preprocessing.
6. Selecting input features and target variable.
7. Analysing class distribution.
8. Splitting data into training, validation and testing sets.
9. Understanding the sigmoid function.
10. Building a Logistic Regression model.
11. Model training and hyperparameter tuning.
12. Predicting probabilities and class labels.
13. Generating a confusion matrix.
14. Evaluating model performance.
15. Calculating classification metrics.
16. Comparing the model with a majority-class baseline.
17. Analysing different classification thresholds.
18. Visualising model performance.
19. Predicting a new example.
20. Discussing limitations and conclusions.

## 4. Methodology

- **Algorithm:** Logistic Regression
- **Preprocessing:** Median imputation and feature standardisation.
- **Training Data:** 14,091 rows
- **Validation Data:** 4,697 rows
- **Testing Data:** 4,698 rows
- **Selected Regularisation Parameter:** C = 0.01
- **Decision Threshold:** 0.62

A stratified split was used to maintain class proportions across the datasets.

## 5. Model Evaluation Results

The final Logistic Regression model achieved the following results on the test dataset:

| Evaluation Metric | Result |
|---|---:|
| Accuracy | 93.68% |
| Precision | 98.80% |
| Recall | 93.45% |
| Specificity | 94.73% |
| F1-Score | 96.05% |
| ROC-AUC | 0.9714 |

### Confusion Matrix

- True Negative (TN): 791
- False Positive (FP): 44
- False Negative (FN): 253
- True Positive (TP): 3610

### Baseline Comparison

The majority-class baseline achieved 82.23% test accuracy, whereas the Logistic Regression model achieved 93.68%.

This indicates that Logistic Regression performs better than the majority-class baseline.

## 6. Example Prediction

For a new review with the following details:

- Age = 28
- Rating = 5
- Positive Feedback Count = 2

The model estimated a 99.22% probability of recommendation.

**Predicted Class:** 1 – Recommended.

## 7. Project Files

The repository contains the following project files:

- `RCA ACT 2 CIE 2.ipynb` – Jupyter Notebook containing the complete implementation.
- `Womens_Clothing_Selected_Features.csv` – Selected dataset.
- `Activity2_Test_Predictions.csv` – Test predictions.
- `Activity2_Threshold_Comparison.csv` – Threshold comparison results.
- `README.md` – Project documentation.

## 8. Limitations and Ethical Considerations

- The dataset may not represent all clothing customers.
- The target classes are imbalanced.
- The model identifies associations and does not establish causation.
- Rating and positive feedback are review-related features.
- Predictions are probability-based estimates and are not guaranteed outcomes.
- The model should not be used as the sole basis for decisions affecting customers.

## 9. Technologies Used

- Python
- Jupyter Notebook / Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 10. Conclusion

In this activity, Logistic Regression was implemented to solve a binary classification problem using the Women's E-Commerce Clothing Reviews dataset.

The model was evaluated using accuracy, precision, recall, specificity, F1-score, ROC-AUC and a confusion matrix.

The results demonstrate that Logistic Regression performed better than the majority-class baseline on the test dataset.

This activity provided practical understanding of data preprocessing, classification, model evaluation, probability prediction and decision threshold selection.

## 11. GitHub Submission Details

**Student GitHub ID:**
https://github.com/complexiota

**Student Name:** Aditi Balasaheb Pawar

**Roll Number:** AD3270

**Class:** T.Y. B.Tech AI & DS

**Division:** B

---

Submitted as part of CIE 2 – Regression and Classification Algorithms (Academic Year 2026–27).
