+++
showonlyimage = true
draft = false
date = "2017-10-09T18:25:22+05:30"
title = "General Linear Models"
weight = 0
+++

Generalized Linear Models

Linear models are used to predict normally distributed data. But when data is binary or categorical, or count traditional linear regression will not work. General Linear Models (glm()) extend linear framework to data that is non normal. Logistic Regression and Possion Regression are two examples of GLM. 
You can use the following code while substituting the fields specified in the table to get the type of regression you want. You pick the ideal type of regression depending on the data.

-glm(formula, family=family(link=function), data=mydata)

This table shows examples of general linear models one can use in the glm() function:
![alt-text](/portfolio/post6.PNG)

Logistic Regression useful when trying to predict a binary outcome from a number of categorical or continuous predictors (independent variables). - see Keep for code You can use a number of diagnostic plots and functions to assess fit. You want a parsimonious model, meaning that if you can eliminate variables while maintaining the highest possible predictive power - do it. You can compare models with anova(). For generalized linear models, you'll want a chi-square version of this test.  - 

-Robust logistic regression-The glmRob() function in the robust package can be used to fit a robust generalized linear model, including robust logistic regression. Robust logistic regression can be helpful when fitting logistic regression models to data containing outliers and influential observations.

-Multinomial logistic regression-If the response variable has more than two unordered categories (for example, married/widowed/divorced), you can fit a polytomous logistic regression using the mlogit() function in the mlogit package. 

-Ordinal logistic regression-If the response variable is a set of ordered categories (for example, credit risk as poor/good/excellent), you can fit an ordinal logistic regression using the lrm() function in the rms package.

Poisson Regression is used when you have count data as the dependent variable with multiple categorical and numeric predictors. Over dispersion is one problem one can encounter in Poisson. It happens when the variance is greater than Poisson distribution predicts. Negative Binomial regression is one way to deal with over dispersion while dealing with count data.  This family of general linear models will still yield reliable predictions, even when the dependent variable is over-dispersed.

Using a general linear model in the Gamma family with either log link or identity link will allow one to make predictions for a dependent variable that is skewed. It serves as an alternative to performing a loglinear transformation of the data.


