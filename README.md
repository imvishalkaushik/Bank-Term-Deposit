# Bank-Term-Deposit
A machine learning approach to identifying customers of Bank Of Portugal who would subscribe to a term deposit.
## Description of the Data set
The Bank of Portugal has collected a huge amount of data that includes customers profiles of those who have subscribed to term deposits and the ones who did not subscribe to a term deposit. The data includes the following columns.
###### 1 — age (numeric)
###### 2 — job: type of job (categorical: ‘admin.’,’blue-collar’,’ entrepreneur’,’ housemaid’,’ management’,’ retired’,’ self-employed’,’ services’,’ student’,’technician’,’ unemployed’,’ unknown’)
###### 3 — marital: marital status (categorical: ‘divorced’,’ married’,’ single’,’ unknown’; note: ‘divorced’ means divorced or widowed)
###### 4 — education (categorical): ‘basic.4y’,’basic.6y’,’basic.9y’,’ high.school’,’ illiterate’,’professional.course’,’ university. degree’,’ unknown’)
###### 5 — default: has credit in default? (categorical: ‘no’,’yes’,’ unknown’)
###### 6 — balance: average yearly balance, in euros (numeric)
###### 7 — housing: has a housing loan? (categorical: ‘no’,’yes’,’ unknown’)
###### 8 — loan: has a personal loan? (categorical: ‘no’,’yes’,’ unknown’)
###### 9 — contact: contact communication type (categorical: ‘cellular’,’telephone’)
###### 10 — month: last contact month of the year (categorical: ‘Jan’, ‘Feb’, ‘mar’, …, ‘Nov’, ‘Dec’)
###### 11 — day_of_week: last contact day of the week (categorical: ‘mon’,’tue’,’wed’,’thu’,’fri’)
###### 12 — duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y=’no’). Yet, the duration is not known before a call is performed. Also, after the end of the call y is known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.
###### 13 — campaign: number of contacts performed during this campaign and for this client (numeric, includes the last contact)
###### 14 — pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means the client was not previously contacted)
###### 15 — previous: number of contacts performed before this campaign and for this client (numeric)
###### 16 — poutcome: outcome of the previous marketing campaign (categorical: ‘failure’,’ nonexistent’,’ success’)
###### 17 — y — has the client subscribed to a term deposit? (binary: ‘yes’,’ no’)
## Exploratory Data Analysis
## Import Necessary Modules and Libraries
###### import pandas as pd
###### import numpy as np
###### import seaborn as sns
###### import matplotlib.pyplot as plt
## Load the Data set
Our model follows Supervised Learning, which consists in learning the link between two datasets: the observed data X and an external variable y that we are trying to predict, usually called “target
## Outliers
Outliers can mislead the training process of machine learning algorithms takes longer training times, less accurate and poor results
## Visualizing
Visualizing the data set using pair-plot,heat-map also find the correlation between them, barplot and also finding the effect of categorical variables on the target. We have also used Distribution plots like Histogram,etc
## Data Preprocessing
Data Preprocessing includees tasks like :- Data Cleaning , Data Transform , Data Reduction. 
Also using Decision tree for filling the null values in the data set.
## Class Imbalance 
Class Imbalance is a major problem in machine learning classification where there is a disproportionate ratio of observations in each class. In this context, many classification algorithms have low accuracy for the class with the lower ratio. In this we use RandomOverSample for fix the data set from imbalance to balanced data set.
## Splitting the Data Set
As we work with datasets, a machine learning algorithm works in two stages. We have split the data around 20%-80% between testing and training stages.
## TRYING LOGISTIC REGRESSSION 
As it is a binary classification problem, We are using Logistic Regression.
## PERFORMANCE EVALUATION
Using Linear Regression getting Accuracy/Score:-
###### Training Score - 81.49%
###### Test Score - 80.68%
## TRYING DECISION TREE 
Decision tree is a machine learning algorithm based on supervised learning. It uses tree representation to solve the problem in which each leaf node represent the class label and attributes are represented on the internal node of the tree. Decisin Tree uses two different types for selection of root node(attribute selection) :- ID3 & CART.
## PERFORMANCE EVALUATION
Using Decision Tree getting Accuracy/Score:-
###### Training Score - 83.53% 
###### Test Score - 83.00%
## TRYING RANDOM FOREST CLASSIFIER
Random forests or random decision forests are an ensemble learning method for classification & regression and other tasks that operates by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees. Random decision forests correct for decision trees’ habit of overfitting to their training set.
## PERFORMANCE EVALUATION
Using Decision Tree getting Accuracy/Score:-
###### Training Score - 75.38% 
###### Test Score - 75.00%
## TRYING SUPPORT-VECTOR MACHINE
Support-Vector Machines are supervised learning models with associated learning algorithms that analyze data for classification and regression analysis. In this section we used Support-Vector Classifier along with two different kernels- RBF and POLY.
## PERFORMANCE EVALUATION
Using Support-Vector Classifier getting Accuracy/Score:-
###### Training Score - 88.87% 
###### Test Score - 87.61%
## TRYING ADABOOST CLASSIFIER
AdaBoost is one of the first boosting algorithms to be adapted in solving practices. Adaboost helps you combine multiple “weak classifiers” into a single “strong classifier”. Here are some facts about Adaboost! → The weak learners in AdaBoost are decision trees with a single split, called decision stumps.
## PERFORMANCE EVALUATION
Using AdaBoost Classifier getting Accuracy/Score:-
###### Training Score - 80.72% 
###### Test Score - 80.30%
## TRYING GRADIENTBOOST CLASSIFIER
Gradient boosting is a machine learning technique for regression, classification and other tasks, which produces a prediction model in the form of an ensemble of weak prediction models, typically decision trees.
## PERFORMANCE EVALUATION
Using GradientBoost Classifier getting Accuracy/Score:-
###### Training Score - 84.80% 
###### Test Score - 84.01%
## Conclusion
The main goal of this project was to be able to predict which customers would subscribe to a term deposit for Bank Of Portugal. The project uses data collected by the Bank of Portugal that includes customers profiles of those who have subscribed to term deposits and the ones who did not subscribe to a term deposit.



