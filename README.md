# Multi-Linear-Regression

## What Is Multiple Linear Regression (MLR)?

Multiple linear regression (MLR), also known simply as multiple regression, is a statistical technique that uses several explanatory variables to predict the outcome of a response variable. The goal of multiple linear regression is to model the linear relationship between the explanatory (independent) variables and response (dependent) variables. In essence, multiple regression is the extension of ordinary least-squares (OLS) regression because it involves more than one explanatory variable.

## What Multiple Linear Regression Can Tell You

Simple linear regression is a function that allows an analyst or statistician to make predictions about one variable based on the information that is known about another variable. Linear regression can only be used when one has two continuous variables—an independent variable and a dependent variable. The independent variable is the parameter that is used to calculate the dependent variable or outcome. A multiple regression model extends to several explanatory variables.

The multiple regression model is based on the following assumptions:

#### 1.There is a linear relationship between the dependent variables and the independent variables

The first assumption of multiple linear regression is that there is a linear relationship between the dependent variable and each of the independent variables. The best way to check the linear relationships is to create scatterplots and then visually inspect the scatterplots for linearity. If the relationship displayed in the scatterplot is not linear, then the analyst will need to run a non-linear regression or transform the data

#### 2.The independent variables are not too highly correlated with each other

The data should not show multicollinearity, which occurs when the independent variables (explanatory variables) are highly correlated. When independent variables show multicollinearity, there will be problems figuring out the specific variable that contributes to the variance in the dependent variable. The best method to test for the assumption is the Variance Inflation Factor method

#### 3.yi observations are selected independently and randomly from the population

#### 4.Residuals should be normally distributed with a mean of 0 and variance σ

Multiple linear regression assumes that the amount of error in the residuals is similar at each point of the linear model. This scenario is known as homoscedasticity. When analyzing the data, the analyst should plot the standardized residuals against the predicted values to determine if the points are distributed fairly across all the values of independent variables. To test the assumption, the data can be plotted on a scatterplot or by using statistical software to produce a scatterplot that includes the entire model.


The coefficient of determination (R-squared) is a statistical metric that is used to measure how much of the variation in outcome can be explained by the variation in the independent variables. R2 always increases as more predictors are added to the MLR model, even though the predictors may not be related to the outcome variable.

R2 by itself can't thus be used to identify which predictors should be included in a model and which should be excluded. R2 can only be between 0 and 1, where 0 indicates that the outcome cannot be predicted by any of the independent variables and 1 indicates that the outcome can be predicted without error from the independent variables.

When interpreting the results of multiple regression, beta coefficients are valid while holding all other variables constant ("all else equal"). The output from a multiple regression can be displayed horizontally as an equation, or vertically in table form.

## The Difference Between Linear and Multiple Regression
Ordinary linear squares (OLS) regression compares the response of a dependent variable given a change in some explanatory variables. However, a dependent variable is rarely explained by only one variable. In this case, an analyst uses multiple regression, which attempts to explain a dependent variable using more than one independent variable. Multiple regressions can be linear and nonlinear.

Multiple regressions are based on the assumption that there is a linear relationship between both the dependent and independent variables. It also assumes no major correlation between the independent variables.

## What makes a multiple regression multiple?
A multiple regression considers the effect of more than one explanatory variable on some outcome of interest. It evaluates the relative effect of these explanatory, or independent, variables on the dependent variable when holding all the other variables in the model constant.

## Why would one use a multiple regression over a simple OLS regression?
A dependent variable is rarely explained by only one variable. In such cases, an analyst uses multiple regression, which attempts to explain a dependent variable using more than one independent variable. The model, however, assumes that there are no major correlations between the independent variables

## Conditions of application


As for simple linear regression, multiple linear regression requires some conditions of application for the model to be usable and the results to be interpretable. Conditions for simple linear regression also apply to multiple linear regression, that is:

1.Linearity of the relationships between the dependent and independent variables should be linear

2.Independence of the observations

3.Normality of the residuals

4.Homoscedasticity of the residuals

Constant variance of the errors should be maintained.

5.No influential points (outliers)

But there is one more condition for multiple linear regression:

6.No multicollinearity:

Multicollinearity arises when there is a strong linear correlation between the independent variables, conditional on the other variables in the model. It is important to check it because it may lead to an imprecision or an instability of the estimated parameters when a variable changes. It can be assessed by studying the correlation between each pair of independent variables, or even better, by computing the variance inflation factor (VIF). The VIF measures how much the variance of an estimated regression coefficient increases, relative to a situation in which the explanatory variables are strictly independent. A high value of VIF is a sign of multicollinearity (the threshold is generally admitted at 5 or 10 depending on the domain). The easiest way to reduce the VIF is to remove some correlated independent variables, or eventually to standardize the data.

## How to choose a good linear model?

A model which satisfies the conditions of application is the minimum requirement, but you will likely find several models that meet this criteria. So one may wonder how to choose between different models that are all valid?

The three most common tools to select a good linear model are according to:

1.The p-value associated to the model,

2.the coefficient of determination R^2 and

## Dummy Variable:

As we know in the Multiple Regression Model we use a lot of categorical data. Using Categorical Data is a good method to include non-numeric data into the respective Regression Model. Categorical Data refers to data values that represent categories-data values with the fixed and unordered number of values, for instance, gender(male/female). In the regression model, these values can be represented by Dummy Variables. 
These variables consist of values such as 0 or 1 representing the presence and absence of categorical values. 

![image](https://user-images.githubusercontent.com/109084435/192427263-65d079ac-46e4-4236-8ef9-6a2110f29147.png)

## Dummy Variable Trap:

The Dummy Variable Trap is a condition in which two or more are Highly Correlated. In the simple term, we can say that one variable can be predicted from the prediction of the other. The solution of the Dummy Variable Trap is to drop one of the categorical variables. So if there are m Dummy variables then m-1 variables are used in the model. 

## Steps Involved in any Multiple Linear Regression Model
#### Step #1: Data Pre Processing 

1.Importing The Libraries.

2.Importing the Data Set.

3.Encoding the Categorical Data.

4.Avoiding the Dummy Variable Trap.

5.Splitting the Data set into Training Set and Test Set.

#### Step #2: Fitting Multiple Linear Regression to the Training set 

#### Step #3: Predicting the Test set results.
