# Credit_card_fraud_detection

## Problem Statement:
The Credit Card Fraud Detection Problem includes modeling past credit card transactions with the knowledge of the ones that turned out to be a fraud. This model is then used to identify whether a new transaction is fraudulent or not. Our aim here is to detect 100% of the fraudulent transactions while minimizing the incorrect fraud classifications. 
There are a lot of fraud happening these these days specially credit card fraud, so we have to build a model which can easily detect fraud transaction with high accuracy and other parameters.

## Understanding and Defining Fraud
Credit card fraud is any dishonest act and behaviour to obtain information without the proper authorization from the account holder for financial gain. Among different ways of frauds, Skimming is the most common one, which is the way of duplicating of information located on the magnetic strip of the card. Apart from this, the other ways are:

* Manipulation/alteration of genuine cards
* Creation of counterfeit cards
* Stolen/lost credit cards
* Fraudulent telemarketing

## Dataset Used
So the dataset name credit_card.csv is taken from the [Kaggle website](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## Techniques Used
The Linear Regression model is used as the data is a binary data which has can predict between two values , Legit or Fraud Transactions. 
* The data is extracted from Kaggle and import all the dependencies and Understand the data. This step is called as Data Collection.
* Since there are no null values in the data set we dont need to Imputation, but counting the value , we get the data to be highly unbalanced. Using the concept of Undersampling , balance the data. Data standardization also be undertaken at this stage. This is called Data Preprocessing and Data Analysis.
* Split the data into features and labels, then split the features and labels data into 4 arrays for training and testing.
* Using the training data train the Linear Regression Model. This step is called Model Fitting.
* Finding the accuracy, precision, recall , confusion matrix and ROC curve and determining the goodness of the model. This step is called as Model Evaluation.
