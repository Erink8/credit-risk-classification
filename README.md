# credit-risk-classification
Machine learning techniques were used to analyze a dataset of lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
## Overview of the Analysis
This challenge included the following steps:
 1. Split the Data into Training and Testing Sets
 2. Create a Logistic Regression Model with the Original Data
 3. Predict a Logistic Regression Model with Resampled Training Data
 4. Write a Credit Risk Analysis Report
### Split the Data into Training and Testing Sets
I first read in our lending_data.csv and created our original dataframe.

I began by separating the columns in the original dataframe and created (y) from the "loan_status" column and (X) from all remaining columns. "0" is assigned to 75,036 values of the "loan_status" column identified as healthy, while "1" is assigned to 2,500 values of the "loan_status" column identified as high-risk. Once the values were identified I was able to split the data using train_test_split. Once split, values for X_train, X_test, y_train, y_test allowing for an initial logistic regression model.

### Create a Logistic Regression Model with the Original Data
Using X_train and y_train I fit the data to a logistic regression model. Next, I used the testing feature data(X_test) and fit the model. To evaluate the model's performance I checked the following:
- Calculate the accuracy score of the model.
- Generate a confusion matrix.
- Print the classification report.
<img width="655" alt="Screenshot 2023-05-21 at 11 44 07 AM" src="https://github.com/Erink8/credit-risk-classification/assets/119360371/699f9a5d-24fd-4f80-a89c-79c410a35b65">

### Predict a Logistic Regression Model with Resampled Training Data
Next, I imported the RandomOverSampler module from imblearn and fit it to the original training dataset. I then fit the sampleted data to logistic regression model. To evaluate the sampled model's performance I checked the following:
- Calculate the accuracy score of the model.
- Generate a confusion matrix.
- Print the classification report.
<img width="830" alt="Screenshot 2023-05-21 at 11 50 33 AM" src="https://github.com/Erink8/credit-risk-classification/assets/119360371/6b8c75a4-b70b-4b3b-9785-5bd4f7521d9e">

## Conclusion
Overall, Model 2 performs with a higher rate of percision and recall than Model 1 for high-risk loans but with less percision and recall for healthy loans. But with the difference of percision and recall being .1 for healthy loans and higher rate of accurancy for high-risk loans, Model 2 is overall more realiable for predicting credit risk.
