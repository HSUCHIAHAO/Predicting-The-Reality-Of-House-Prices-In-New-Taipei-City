# group-project-group-r

# Predicting The Reality Of House Prices In New Taipei City

The data source:https://data.gov.tw/dataset/125903

### Summary

#### Purpose

This proposal will show the audience of our plan to analyze the reality values in New Taipei City . We
will try to predict the realty price for the future which is based on the present price, and predict which
area in Reality will cover more values. About Reality, we also call it real estate or real property, in our
assignment, reality we refer in particular to houses, apartments and other buildings which can let
people work or live in. The reason that we choose Taiwan is we are familiar with it and we will face
the problems that we will be able to solve in our assignment in the future.

#### Background

Reality is a very popular topic in recent years, people always choose to purchase reality for investment
or daily use. Unfortunately, As graduate students, we need to face the question about the reality of
prices in the next few years.

### Discussion

#### Techniques

We expect to use simple linear regression, xgbregressor, and polynomialfeatures in our analysis. To
predict a value, we should use several algorithms to know what kinds of features will result in high
prices.

#### Description Goal

R square > 0.75
We wish that the R square can be higher than 0.75 because it is good evidence that the model is
suitable for everyone to know the price by many features.

#### Dataset

The datasets that we download from Taiwan government open data website. The format of the dataset
is in csv. There are 3,637 rows and 26 columns in the dataset. Because many cities have very different
price intervals, we choose the dataset that houses are from New Taipei city.

#### Translate language and Save new dataset

The language in this dataset is Chinese, so we need to spend a lot of time translating the language
from Chinese to English. When we finish the following work, we need to save a new csv file for us to
start our project.

#### Data Cleaning

##### 1. Detecting Null Values

Cleaning data is a rough task, if we do not have a good dataset to train, the performance would be
affected seriously. Detecting null value is the first step that is very important.

##### 2. Dealing With Null Values

There are several ways to deal with null values. For example, filling null value with mean, median, or
mode. It is fine to drop the row with null value, but sometimes it depends on the type of dataset. We
should carefully deal with null value in each column.
#### Plan


● Data exploring
To find the trend in each column, it is basic to visualize the data. Sometimes, it is
necessary to compare many attributes like correlation matrix. It helps us to know
more about the data.

● Feature engineering
In reality, there are too many variables, so we need to condense them to make the
regression become much simpler. Sometimes, the variable is category, and we can use
one-hot encoding to keep the important variable in the dataset.


● Choose independent variables
Pick those ideal independent variables for response in training and testing

● Dataset splitting training and testing dataset
For predicting the data, we need to split the dataset. It is fine to split the dataset into
80%(training data) and 20%(testing data).

● Choose algorithms
Creating a linear model to make a linear regression.

● fit testing X, testing Y & fit testing Y, prediction Y
We need to make sure the performance is well before we fit the testing and
prediction. If the performance (R square, MSE) is pretty low, we should go back to
the step of feature engineering and re-select the new independent variables.
If the R square has a huge difference in the model, it is called overfitting, and we need
to go back to the step of feature engineering to improve the R square.
