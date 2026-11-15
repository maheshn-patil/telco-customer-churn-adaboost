# telco-customer-churn-adaboost
# Telco Customer Churn Prediction Using AdaBoost
# MINOR PROJECT
## Telco Customer Churn Prediction Using AdaBoost

**Student Name:** Maheshagouda N Patil

**Dataset Name:** Telco Customer Churn

**Course/Batch:** Artificial Intelligence ,Batch October

**Kaggle Link:** [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---
## 1. Project Overview

This project focuses on predicting customer churn in a telecommunications company using Machine Learning.

Customer churn refers to customers leaving a company's services. The project uses the AdaBoost classification algorithm to predict whether a customer is likely to leave or stay.

## 2. Dataset

* **Dataset:** Telco Customer Churn
* **Source:** [Kaggle – Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
* **Total Records:** 7,043
* **Total Columns:** 21
* **Target Variable:** Churn

The dataset contains customer information, subscribed services, contract details and billing information.

## 3. Technologies Used

* Python
* Google Colab
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

## 4. Project Workflow

1. Dataset collection and loading
2. Data understanding and inspection
3. Data cleaning and preprocessing
4. Exploratory Data Analysis (EDA)
5. Feature encoding
6. Training and testing data splitting
7. AdaBoost model training
8. Model evaluation
9. Feature importance analysis

## 5. Data Preprocessing

* Checked missing values and duplicate records.
* Converted `TotalCharges` into numerical format.
* Replaced 11 missing `TotalCharges` values with zero because those customers had zero tenure.
* Removed the `customerID` column.
* Converted categorical features using One-Hot Encoding.
* Split the dataset into 80% training and 20% testing data.

## 6. Machine Learning Algorithm

**AdaBoost (Adaptive Boosting)** was used for customer churn classification.

A Decision Tree with maximum depth 1 was used as the weak learner.

Model parameters:

* Number of estimators: 50
* Learning rate: 1.0
* Maximum tree depth: 1

## 7. Model Results

| Evaluation Metric | Result |
| ----------------- | -----: |
| Accuracy          | 80.06% |
| Churn Precision   |   0.64 |
| Churn Recall      |   0.56 |
| Churn F1-score    |   0.60 |
| ROC-AUC           |   0.84 |

## 8. Important Findings

* Month-to-month contracts had the highest feature importance.
* Customer tenure was the second most important feature.
* Customers with shorter tenure generally showed higher churn.
* Customers who left generally had higher monthly charges.

## 9. Conclusion

The AdaBoost model achieved 80.06% accuracy and an ROC-AUC score of 0.84 on the test dataset. The project demonstrates how Boosting techniques can be applied to predict customer churn.

The model can be further improved by experimenting with different parameters and techniques to increase churn recall.

## 10. Future Improvements

* Improve the identification of customers likely to leave.
* Experiment with other Boosting algorithms.
* Perform additional hyperparameter tuning.
* Deploy the model through a simple web application.
