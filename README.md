# Credit-Risk-Classification

##Instructions

### Split the Data into Training and Testing Sets

1. **Read the Data:**
   - Read the "lending_data.csv" data from the Resources folder into a Pandas DataFrame.

2. **Create Training and Testing Sets:**
   - Created the labels set (y) from the “loan_status” column.
   - Created the features (X) DataFrame from the remaining columns.
   - Checked the balance of the labels variable (y) using the `value_counts` function.
   - Split the data into training and testing datasets using `train_test_split`.

### Created a Logistic Regression Model with the Original Data

1. **Fit a Logistic Regression Model:**
   - Fit a logistic regression model using the training data (X_train and y_train).
   - Saved the predictions on the testing data labels using the testing feature data (X_test) and the fitted model.

2. **Evaluate Model Performance:**
   - Calculate the accuracy score of the model.
   - Generate a confusion matrix.
   - Print the classification report.
   - Answer the question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

### Predict a Logistic Regression Model with Resampled Training Data

1. **Resample the Data:**
   - Use the RandomOverSampler module from the imbalanced-learn library to resample the training data.

2. **Fit Logistic Regression Model with Resampled Data:**
   - Use the LogisticRegression classifier and the resampled data to fit the model and make predictions.

3. **Evaluate Model Performance on Resampled Data:**
   - Calculate the accuracy score of the model.
   - Generate a confusion matrix.
   - Print the classification report.
   - Answer the question: How well does the logistic regression model, fit with oversampled data, predict both the 0 (healthy loan) and 1 (high-risk loan) labels?


### Analysis

1. **Overview of the Analysis:**
   The purpose of this was to use various techniques to train and evaluate models with imbalanced classes. Used a dataset of historical lending activity from a peer-to-peer    lending services company to build a model that can identify the creditworthiness of borrower.

3. **Summary:**
   The logistic regression model with resampled data shows significantly improved balanced accuracy compared to the model with the original data.
   Both models exhibit high precision and recall for label 0 (healthy loan), but the model with resampled data performs slightly better.
   For label 1 (high-risk loan), both models have high precision and recall, with the resampled data model having a slight edge.
   The resampled data model seems to perform better in terms of balanced accuracy, indicating that it might be a more robust choice for predicting credit risk. However,        further analysis and consideration of specific business requirements are recommended before making a final model selection.
