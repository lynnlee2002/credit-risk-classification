# credit-risk-classification

## 1) Split the Data into Training and Testing Sets
- Open the starter code notebook and use it to complete the following steps:
  + Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
  + Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
  + Split the data into training and testing datasets by using train_test_split.

## 2) Create a Logistic Regression Model with the Original Data
- Fit a logistic regression model by using the training data (X_train and y_train).
- Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
- Evaluate the model’s performance by doing the following:
- Generate a confusion matrix.
- Print the classification report.
- Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

## 3) Write a Credit Risk Analysis Report:
- An overview of the analysis: It helps evaluate the effectiveness of the logistic regression model in predicting healthy (labeled "0") and high-risk loans (labeled "1"). It provides valuable insights for assessing the model's performance and informs decision-making processes in loan classification and risk assessment tasks.
- The results:
  + With the original data:
    --> For the 0 (healthy loan) label: The precision, recall, and f1-score are all 1.00, which means that the model accurately identifies all instances of healthy loans. The precision of 1.00 indicates that when the model predicts a loan as healthy, it is almost always correct. The recall of 1.00 means that the model captures all instances of healthy loans, without missing any.
    --> For the 1 (high-risk loan) label: The precision is 0.87, which means that when the model predicts a loan as high-risk, it is correct around 87% of the time. The recall is 0.89, indicating that the model successfully identifies 89% of the high-risk loans. The F1-score is 0.88, which represents a good balance between precision and recall for the high-risk loan label.
  + With the resampled data:
    --> For the 0 (healthy loan) label: The precision, recall, and f1-score are all 1.00, which means that the model accurately identifies all instances of healthy loans. This indicates that the model performs exceptionally well in predicting healthy loans.
    --> For the 1 (high-risk loan) label: The precision indicates that when the model predicts a loan as high-risk, it is correct approximately 87% of the time.The recall for class 1 is 1.00, indicating that the model correctly captures all instances of high-risk loans. The f1-score for class 1 is 0.93 suggesting that the model performs well in predicting high-risk loans.
- A summary: I would recommend the model performed on the resampled data as the it results in a higher precision and f1-score for the "1" label (high-risk loan), indicating a more accurate performance on predicting/capturing high-risk loans.
