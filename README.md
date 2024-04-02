## credit-risk-classification

### Overview of the Challenge

The objective of this Challenge is to develop a machine learning model that can accurately predict the creditworthiness of borrowers based on historical lending data. 

### Splitting the Data into Training and Testing Sets

I started by reading the lending_data.csv dataset into a Pandas DataFrame and splitting the data into training and testing sets. The labels set (y) was created from the "loan_status" column, while the features set (X) was created from the remaining columns.

### Creating a Logistic Regression Model with the Original Data

I trained a logistic regression model using the training data (X_train and y_train). The model was fitted to the training data and used to make predictions on the testing data (X_test). I evaluated the model's performance by generating a confusion matrix and printing a classification report.

### Evaluation of the Model's Performance

The logistic regression model demonstrated strong performance in predicting credit risk:
- **Confusion Matrix:** The confusion matrix showed that the model correctly classified a large majority of loans as healthy (0) or high-risk (1).
- **Classification Report:** The classification report provided detailed metrics such as precision, recall, and F1-score for both healthy and high-risk loans.

## Credit Risk Analysis Report

### Overview of the Analysis

In this analysis, we aimed to build a machine learning model to predict the creditworthiness of borrowers using historical lending data from a peer-to-peer lending services company. The purpose of this analysis was to develop a model that could accurately classify loans into healthy and high-risk categories based on various financial features. We focused on the "loan_status" column as our target variable, with values of 0 indicating a healthy loan and 1 indicating a high-risk loan.

We started by reading the lending_data.csv dataset into a Pandas DataFrame and then split the data into features (X) and labels (y). We used logistic regression, a popular classification algorithm, to build the predictive model. The logistic regression model was trained on the training data (X_train and y_train) and evaluated using the testing data (X_test and y_test). Finally, we generated a confusion matrix and a classification report to assess the model's performance.

### Results

**Logistic Regression Model:**
- **Accuracy:** 0.99
- **Precision (High-risk loans):** 0.85
- **Recall (High-risk loans):** 0.91

### Summary

The logistic regression model performed exceptionally well in predicting credit risk, achieving an accuracy score of 0.99. The precision score for high-risk loans indicates that 85% of the loans predicted as high-risk were correctly classified among all predicted high-risk loans. Additionally, the recall score for high-risk loans suggests that the model correctly identified 91% of the actual high-risk loans among all actual high-risk loans.

Based on the evaluation metrics, we recommend deploying the logistic regression model for credit risk assessment. The model demonstrates strong performance in identifying high-risk loans, which is crucial for mitigating potential losses associated with defaults. However, it's essential to consider the problem context and business objectives when evaluating model performance. For example, the importance of predicting high-risk loans accurately may vary depending on the company's risk tolerance and strategic goals.

Overall, the logistic regression model offers a reliable solution for credit risk assessment and can significantly contribute to improving the company's decision-making process in loan approvals.
