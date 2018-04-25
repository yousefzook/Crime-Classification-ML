# San Fransisco Crime Classification Problem
## For Udacity Machine Learning Capstone Project

## Problem Statement:
From 1934 to 1963, San Francisco was infamous for housing some of the
world's most notorious criminals on the inescapable island of Alcatraz.
Today, the city is known more for its tech scene than its criminal past. But,
with rising wealth inequality, housing shortages, and a proliferation of
expensive digital toys riding BART to work, there is no scarcity of crime in
the city by the bay.

From Sunset to SOMA, and Marina to Excelsior, this competition's dataset
provides nearly 12 years of crime reports from across all of San Francisco's
neighborhoods. This is a multi-class classification problem, given time and
location, the goal is to predict the category of crime that occurred.

## Data
You can download data sets from kaggle link:
https://www.kaggle.com/c/sf-crime/data

## Metrics:
This problem contains imbalanced data, so metrics like accuracy will not work well with the data, istead we will use [LogLoss](http://wiki.fast.ai/index.php/Log_Loss) and [Fscore](https://en.wikipedia.org/wiki/F1_score) as our metrics.

## Algorithms and Techniques:
There are 7 algorithms used in this problem and compared together.
* Naive random predictor
* [DecisionTreeClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
* [MLPClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html)
* [XGBClassifier](http://xgboost.readthedocs.io/en/latest/python/python_api.html)
* [KNeighborsClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
* [SVClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)
* [ExtraTreesClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.ExtraTreesClassifier.html)

## Results:
The best algorithm in terms of logloss is SVClassifier but it takes huge time in training.
ExtraTreesClassifier is the also good but need huge amount of resources especially memory.
The chosen algorithm is MLPClassifier as it is the most suitable one
Final score = 2.67607
