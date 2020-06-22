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
 
 In this project, 
 -I did exploratory data analysis to gain understanding about the different variables in the given dataset. 
