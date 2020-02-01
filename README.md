# Predicting Credit Card Fraud Detection
The datasets contains transactions made by credit cards in by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, all feature names are not provided. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, Accuracy is measured using the Area Under the Precision-Recall Curve (AUPRC).

 - Used xgboost library for classification.
 - xgboost random forest worked quite well with this classification and gave around 85% accuracy.
 - During 10-fold cross-validation, accuracy stood at 83%.
 
 As git hub is not allowing to upload files larger than 100MB, I am adding dataset url here:
 https://www.kaggle.com/mlg-ulb/creditcardfraud
 
 Download "creditcard.csv" from there and keep it along with jupyter notebook.