## Introduction

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this project, I will build the predictive model that answers the questions: "what sorts of people were most likely to survive?" using passenger data.

## Problem Statment

Predict the survival of Titanic passengers.

## Data Description

I have downloaded the dataset for this problem from https://www.kaggle.com/c/titanic/data

The data has been split into two groups:

 - training set (train.csv)
 - test set (test.csv)
 
The training set is used to make machine learning models and evaluation. The test set is used to see how well your model performs on the unseen data.

The traning data contains the following columns:

 - survival     Survival            0 = No, 1 = yes
 - pclass       Ticket Class        1 = 1st, 2 = 2nd, 3 = 3rd
 - sex          Sex
 - Age          Age in years
 - sibsp        # of siblings/spouses aboard the Titanic
 - parch        # of parents/children aboard the Titanic
 - ticket       Ticket Number
 - fare         Passenger fare
 - cabin        Cabin Number
 - embarked     Port of Embarkation    C = Cherbourg, Q = Queenstown, S = Southampton
 
 ## Methodology
 
 In this project First I did exploratory data analysis to gain understanding about the different variables in the given dataset. 
 ### Findings from Exploratory Data Analysis
    - There are more number of males than the females in the training set.
    - More Passengers died and less survived.
    - More females survived and less males survived.
    - Passengers from the 1st class survived more.
  
 In Feature PreProcessing, I handled the missing values by replacing with mean and most frequent value. To handle the categorical data I did one hot encoding.
 
 After cleaning the data and making it ready for the machine learning algorithm, I trained various models and evaluated them using the k-fold cross validation. Since some of the models were giving the nearly same cross_val_score, i have also calculated auc to select the best model for making predictions on the test set.
 The models which I have trained are the following:
 - Logistic Regression
 - Decision Tree Classifier
 - Support Vector Classifier
 - KNeighbors Classifier
 - Random Forest Classifier
 - Voting Classifier
 - Bagging Classifier
 - AdaBoost Classifier
 - GradientBoosting Classifier
 
 After training and evaluating these models, I selected the Voting Classifier as the final model and made the predictions on the test set using this Classifier.
