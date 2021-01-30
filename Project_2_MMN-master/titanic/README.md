# Project2 -  Kaggle Challenges with Titanic Survival - Classification, and House Prices - Regression
## Part 2: Titanic - Machine Learning from Disaster

![alt text](https://impm.org/wp-content/uploads/2020/04/titanic.jpg)

<b>Team numbers: 10 
 
Team members:  Maha Aldosary - Noha Zamaan- Mariah Alshiekh(leader)</B>

## Table of contents
* [overview](#overview)
* [Define the problem](#Define-the-problem)
* [Data-sets Description](#Data-sets-Description)
* [Technologies](#technologies)
* [Methodology](#methodology)
* [Outcome](#Outcome)


---

## overview

This is our second project with GA (General Assmply) on DSI(Data Sience Imperssive) course.
In this project, we participated in the challenge presented on Kaggle platform. The main aim of this project is Searching for the best prediction for people has more chance of survival, depending on the Titanic dataset.

## Define the problem
 “what sorts of people were more likely to survive?”
Titanic data has verity of features that describe the satuation in titanic ship. most of these features have object type. 
So, classification model works perfectly with these data and we applied multiable kind of classfication model in order to select the model that provide best score.

---

## Data-sets Description

[train_data: ](https://www.kaggle.com/c/titanic/data?select=train.csv)will contain the details of a subset of the passengers and importantly, will reveal whether they survived or not, also known as the “ground truth”.

[test_data:](https://www.kaggle.com/c/titanic/data?select=test.csv) dataset contains similar information but does not disclose the “ground truth” for each passenger. 

|Feature|Type|Description|
|---|---|---|
|PassengerId|int64|ID
|survival|int64|Survival	0 = No, 1 = Yes|
|pclass|int64|Ticket class	1 = 1st, 2 = 2nd, 3 = 3rd|
|Name|object|Passenger name|
|sex	| object       |Sex	|
|Age	|float64|Age in years	|
|sibsp|int64| of siblings / spouses aboard the Titanic	|
|parch|int64|of parents / children aboard the Titanic	|
|ticket|object|Ticket number	|
|fare|float64|	Passenger fare	|
|cabin|object|	Cabin number	|
|embarked|object|	Port of Embarkation	C = Cherbourg, Q = Queenstown, S = Southampton|


## Technologies
I worked on : 
* mac OSx64 
* Anaconda-Navigator version3 
* python version 3.9.0 
* Jupyter notebook version 6.1.4
* githup version 2.6.0


## Methodology
In this Project we We Worked on three strategies :

1- First stratiges : Fill missing value with (mean and mod) method [here](https://www.kaggle.com/mariahalshiekh/project-taitanic)

2- Second stratiges: Fill missing value using Random Foreset [here](https://www.kaggle.com/mariahalshiekh/project-titanic-rf-clean)

3- Third stratiges : Fill missing value using Knn classifier [here](https://www.kaggle.com/mariahalshiekh/project-taitanic-knn-clean)

with all these stratiges we trained our data on 6 models:

* Logistic-Regression
* Knn-Classifier
* Decision Tree
* Bagging classifier
* Random Forest
* Extra Trees

And we trying to optomizing our model by using `pipline` and `Grid Search`

## Outcome
- In First strategie we reached to highest scorse on testing data by using `Random Forest` classifier with `Grid Search` which equals = 0.7723
- In second strategie we reached to highest scorse on testing data by using `Decision-Trees` classifier with `Grid Search` which equals = 0.7870
- In Third strategie we reached to highest scorse on testing data by using ` Extra-Trees with ` which equals = 0.7775	

So, To reache to highest score on test dataset we should fill missing value using `Random Forest` and fit `Decision-Trees` model using
 `Grid Search`
