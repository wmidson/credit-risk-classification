# credit-risk-classification

## Instructions

The instructions for this Challenge are divided into the following subsections:

  * Split the Data into Training and Testing Sets

  * Create a Logistic Regression Model with the Original Data

  * Predict a Logistic Regression Model with Resampled Training Data

  * Write a Credit Risk Analysis Report

### Split the Data into Training and Testing Sets

Open the starter code notebook and use it to complete the following steps:

1. Read the `lending_data.csv` data from the Resources folder into a Pandas DataFrame.

2. Create the labels set (`y`) from the “loan_status” column, and then create the features (`X`) DataFrame from the remaining columns.

3. Split the data into training and testing datasets by using train_test_split.

### Create a Logistic Regression Model with the Original Data

Use your knowledge of logistic regression to complete the following steps:

1. Fit a logistic regression model by using the training data (`X_train` and `y_train`).

2. Save the predictions for the testing data labels by using the testing feature data (`X_test`) and the fitted model.

3. Evaluate the model’s performance by doing the following:
    * Calculate the accuracy score of the model.
    
    * Generate a confusion matrix.

    * Print the classification report.

4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

##  Overview of Analysis
* Purpose: Create a model that can identify the creditworthiness of borrowers
* Resources: csv data set that included historical lending activity from a lending services company
* Dependent Variable: (y value) - "loan status". Shows whether a loan is healthy (0) or high-risk (1) . 
* Independent variables: (X values) - "loan size", "interest rate", "borrower income", "debt to income ratio", "number of accounts", and "derogatory marks".

## Process
1. Read in lending_data.csv data from resources folder into a DataFrame
2. Split the data into training and test sets for x's and y's using train_test_split (X_test, X_train, y_test, y_train)
3. Defined the dependent and independent variables
4. Created logistic regression model from the original data
5. Fitted logistic regression model using the training data (X-train, y_train) and made predictions
6. Evaluated the model's performance

## Results
The model predicted healthy loans at 100% precision and high risk loans at 84% precision. 

## Summary 
Collected data can be used effectively to create a functioning machine learning model. Randomly oversampling data allows for blanaced accuracy and high recall scores, which allow the model to predict high risk loans more effectively. 
The model with original data was less likely to predict false negatives than the model using oversampled data (false negative = low risk when in reality high risk). 
The Model with randomly oversampled data is likely the best model to use based on the high accuracy and recall values. I would recommend it. 
