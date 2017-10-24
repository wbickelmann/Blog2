+++
showonlyimage = true
draft = false
date = "2017-10-23T18:25:22+05:30"
title = "Linear Discriminant Analysis"
weight = 0
+++

Linear Discriminant Analysis

LDFA is a linear classifier which classifies observations based on a linear combination of variables. It searches for the combination which separates the variables most effectively. Unlike many other methods, Linear discriminant analysis, models the predictor variable distribution instead of the dependent variable. The algorithm uses the model to take a Bayesian approach to make an estimate for Pr(Y = k|X = x). This method should be used when the predictor variables have a normal distribution, when the classes are clearly separated.   It is also more popular than logistic regression when these conditions are met and when there are more than two classes.

Advantages of Linear discriminant analysis are that it can take a small sample size, unlike logistic regression, and that it also has a relatively low variance, since it is restrictive model compared to LDFA. However, this also means that it can suffer from higher bias, thus contributing to error. It is also useful when classifying into more than 2 classes. It assumes equal covariance matrices across predictors and a gaussian distribution. However it can lead to overfitting. LDA accepts continuous input for predictor variables and classifies nominal or ordinal data for a response variable.

Visualizing LDFA is fairly simple when you are dealing with a two-dimensional plane as seen below. You are just separating the classes with a linear decision boundary

