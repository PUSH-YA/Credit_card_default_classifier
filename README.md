# Credit card default classifier
Supervised machine learning model for classifying clients who will defaul or not based on their past transactions and some client information

## Preprocessing
The model is first split into training and testing data, there is some minor EDA done on the dataset to understand the problem set better, A preprocessor transformer is created for the data set which is then used for multiple ML model pipelines. 

## Machine learning models
First a baseline classifier dummy model is created for predicting based on the most frequent class available. 
A logistic regression model is first fit onto the model and then several non-linear models (k-nn classifier, SVC with linear and rbf kernel, and random forest classifier) is created. Hyperparameter optimisation is perforemd on all the models using GridSearchCV and RandomisedSearchCV.

## Feature selection
Forward feature is used to select the most important features for the model. A logisitc regression model is used for selecting the features in the forward feature selection algorithm

## Hyperparameter optimisation
Hyperparameter optimisation is perforemd on all the models using GridSearchCV and RandomisedSearchCV (where exhaustive grid search would be too inefficient and time consuming).

## Testing the model
The model is finally tested on the test data set and evaluated according to classification metrics such as precision, recall and f1 score.
