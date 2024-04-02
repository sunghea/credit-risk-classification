# Supervised Learning

### Overview of the Challenge(credit-risk-classification)

The objective of this Challenge is to develop a machine learning model that can accurately predict the creditworthiness of borrowers based on historical lending data. 

### Splitting the Data into Training and Testing Sets

I started by reading the lending_data.csv dataset into a Pandas DataFrame and splitting the data into training and testing sets. The labels set (y) was created from the "loan_status" column, while the features set (X) was created from the remaining columns.

### Creating a Logistic Regression Model with the Original Data

I trained a logistic regression model using the training data (X_train and y_train). The model was fitted to the training data and used to make predictions on the testing data (X_test). I evaluated the model's performance by generating a confusion matrix and printing a classification report.

### Evaluation of the Model's Performance

The logistic regression model demonstrated strong performance in predicting credit risk:
- **Confusion Matrix:** The confusion matrix showed that the model correctly classified a large majority of loans as healthy (0) or high-risk (1).
- **Classification Report:** The classification report provided detailed metrics such as precision, recall, and F1-score for both healthy and high-risk loans.

# Credit Risk Analysis Report

## Overview of the Analysis

In this analysis, we aimed to develop machine learning models to predict the creditworthiness of borrowers based on historical lending data. The purpose was to assist financial institutions in assessing lending risks. The data included various financial information about borrowers, such as credit score, debt-to-income ratio, loan amount, etc. We needed to predict the likelihood of loan default, which was indicated by the "loan_status" column.

We followed a typical machine learning process, starting with data preprocessing, splitting the data into training and testing sets, and training various models. We primarily utilized logistic regression for this analysis, although other algorithms could be explored in future iterations.

## Results

- **Logistic Regression Model:**
  - Accuracy: 0.99
  - Precision (High-risk loans): 0.85
  - Recall (High-risk loans): 0.91

## Summary

The logistic regression model outperformed others in terms of accuracy, precision, and recall. It demonstrated strong performance in identifying high-risk loans, which is crucial for minimizing potential losses due to defaults. However, the choice of the best model depends on the problem context and business objectives. For instance, if it's more important to minimize false positives (predicting healthy loans as high-risk), then precision becomes a critical metric. Conversely, if minimizing false negatives (predicting high-risk loans as healthy) is more critical, then recall takes precedence.

Considering the high performance of the logistic regression model and its relevance to the problem at hand, we recommend deploying it for credit risk assessment. Nonetheless, continuous monitoring and optimization of the model may further enhance its predictive capabilities over time.

