# credit-risk-classification
Module 20 Supervised Learning

## Overview of the Analysis

In this analysis, the goal was to build and evaluate a machine learning model to predict loan risk based on historical lending data from a peer-to-peer lending services company. The primary objective was to develop a model capable of identifying the creditworthiness of borrowers.

**Purpose of the Analysis:** The purpose of the analysis was to assess the credit risk associated with loans by leveraging machine learning techniques. The goal was to create a model that could effectively classify loans into two categories: healthy loans (0) and high-risk loans (1).

* **Financial Information:** The dataset, sourced from the "lending_data.csv" file, contained various financial attributes related to loan transactions. The target variable for prediction was the "loan_status" column, where a value of 0 indicated a healthy loan, and a value of 1 indicated a high risk of default.

**Variables to Predict:** The variable of interest was the "loan_status" column, representing the credit risk associated with each loan. The analysis aimed to predict whether a loan falls into the category of healthy or high-risk.

**Stages of the Machine Learning Process:**
1. **Data Preprocessing:** Reading the dataset, creating labels and features, and splitting the data into training and testing sets.
2. **Model Selection:** Utilizing logistic regression for credit risk prediction.
3. **Training and Testing:** Fitting the logistic regression model using training data and evaluating its performance on testing data.
4. **Evaluation:** Generating a confusion matrix and printing a classification report to assess the model's accuracy, precision, and recall.

**Methods Used:** 
- Logistic Regression: Selected as the machine learning algorithm for credit risk classification.
- Train-Test Split: The dataset was divided into training and testing sets to train and evaluate the model.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Precision, Recall, and F1-Score are all high for both classes (0 and 1). This indicates that the model is performing well in terms of both precision (how many predicted high-risk loans are actually high-risk) and recall (how many actual high-risk loans were correctly predicted).
  * Balanced accuracy score: 95.20%
  * Precision, recall, and f1-score are high for both classes. The model performs well in distinguishing healthy and high-risk loans.

* Machine Learning Model 2:
  * The high precision suggests that there is a low false positive rate. The high recall suggested there is a low false negative rate. The F1 score suggests there is a good balancce between precision and recall for both classes. Overall accuracy is 99% which suggests a strong overall performance.
  * Balanced accuracy score: 99.47%
  * Similar high performance as Model 1, indicating effective handling of class imbalance through oversampling.

## Summary

Both models demonstrate strong performance. Given that the priority is predicting the creditworthiness of borrowers, the model's effectiveness in correctly identifying high-risk loans (label 1) is of high importance.

Model 1 (Original Data):

Balanced accuracy score: 95.20%
Precision (label 1): 0.85
Recall (label 1): 0.91

Model 2 (Oversampled Data):

Balanced accuracy score: 99.47%
Precision (label 1): 0.99
Recall (label 1): 0.99 

My recommendation would be Model 2 (oversampled data). This is because it shows a higher precision and recall for high-risk loans (the 1's) which suggests it has the edge in identifying borrowers at risk of defaulting on their loans. This also means it is more likely to identify creditworthy borrowers which aligns with the main objective of the model. Therefore, Model 2 should be the preferred choice.
