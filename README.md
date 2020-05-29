# mod3_project
# Preventing Churn in the Telecom Industry

## Problem
Why do consumers leave your telecom carrier and how can we prevent it?

## The Process
1. Gather The Data 
2. Perform extensive Exploratory Data Analysis to get a better understanding 
3. Feature Engineering and Selection
4. Modeling and Making predictions 
5 .Evaluate and offer insight

## The Data 
Telecom consumer data set  from Kaggle
Data set contains 3,333 rows and 21 columns
Columns include information about the consumers and rows are each consumer
Ex. State, type of plan, and how many calls the consumer makes.

## EDA 
Charge Per Minute - Charge / Minutes
    Proved to be very helpful in determining why consumers might leave.
    International had the highest charge per minute with 0.27
    Day had an average of 0.17
    Night had the lowest at 0.045
    * All rows had similar rate showing the company has a flat rate for each call
Churn(target variable)-Very Large Class Imbalance 
2,850 consumers do not churn
483 consumers churn
Churn rate is 14.5%

Correlation- As you can see, charge and minutes are directly correlated for each type of call
Churn a high correlation with total day minutes of 0.2
Churn also has a high correlation with customer service calls at 0.2

## Feature Selection
Tried 3 different approaches for categorial data:
Dummy Variables 
Factorize Variables
Label Encoder
*Dummy Variables worked the best

## Class Imbalance
Resampled 
Smote

## Best Models
XGBoost With Gridsearch
Random Forest With GridSearch
Decision Tree Classifier With Gridsearch

## Takeaways
Strongest features were total day, eve, and night, minutes.

## Recommendations
Lower the charge on day minutes because the people that talked the most during the day were the most likely to Churn

Either get rid of or improve the International Plan as most of the consumers with it Churned

Improve Customer Service and try to help them quickly to limit the customer service calls

## Furthur Research
Would like to lower the Threshold to have higher recall score and limit false negatives 



