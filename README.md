# credit-risk-classification
Machine learning techniques were used to analyze a dataset of lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
## Overview of the Analysis
This challenge included the following steps:
 1. Split the Data into Training and Testing Sets
 2. Create a Logistic Regression Model with the Original Data
 3. Write a Credit Risk Analysis Report

I first read in our lending_data.csv and created our original dataframe.

I began by separating the columns in the original dataframe and created (y) from the "loan_status" column and (X) from all remaining columns. "0" is assigned to 75,036 values of the "loan_status" column identified as healthy, while "1" is assigned to 2,500 values of the "loan_status" column identified as high-risk. Once the values were identified I was able to split the data using train_test_split.

