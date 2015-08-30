# List of Common Machine Learning Algorithms



_d</em></p>bug_@jessefish.net</article></div>tester

This is an instructional file to explain common machine learning
algorithms and how to implement them using R and Python. 

Below is a list of common machine learning algorithms. 

* Linear Regression
* Logistic Regression
* Decision Tree
* SVM
* Naive Bayes
* KNN
* K-Means
* Random Forest
* Dimensionality Reduction Algorithms
* Gradient Boost & Adaboost

## Linear Regression

Linear Regression is is an approach for modeling the relationship between a scalar dependent variable y and one or more explanatory variables (or independent variables) denoted X. In other words, an atempt is made to 'fit' a linear equation to the observed data. The case of one explanatory variable is called simple linear regression. Linear Regression is used to estimate real values - the cost of houses, the total number of calls, sum total of sales, etc.  sales - based on one or more continuous variables. 

When using Linear Regression, we establish relationship between independent and dependent variables by fitting a 'best line.' A line of best fit, or best fit line, is also known as regression line. This does not necessarily imply that one variable *causes* the other variable, but that there is some significant association between the two variables. A 'simple' linear regression can be represented by the equation y = a + b * X, where x is the explanatory variable and Y is the dependent variable. The slope of the line is b, and a is the intercept (the value of y when x = 0). If here appears to be no association between the proposed explanatory (i.e. X) and dependent (i.e. y) variables - that is, an increasing or decreasing trend does not appear apparent - then fitting a linear regression model will probably not be a useful model. 

So. What do we mean by all of this? 

Consider the following example. 

Suppose we want to understand how the population of a city can have an effect on the profit of stores within that city. In our first example, let's look at the ex1dat1.txt file within the data folder. The first column repreents the population of the city. The second column is the profit of having a store in that city, and a negative value within the second column indicates profit loss. 

Using Python, let's first look at a visualization of this data (without any regression line applied). We can write the following, which is located within the src folder as linreg.py: 

```
from numpy import loadtxt, zeros, ones, array, linspace, logspace
from pylab import scatter, show, title, xlabel, ylabel, plot, contour



#Load the dataset
data = loadtxt('../ex1data1.txt', delimiter=',')

#Plot the data
scatter(data[:, 0], data[:, 1], marker='o', c='b')
title('Profits distribution')
xlabel('Population of City in 10,000s')
ylabel('Profit in $10,000s')
show()
```

From looking at the output of the data in the form of a scatter plot, it seems obvious that there is a correlation: the larger the population of a city is, the more a store will make in profit. But let's find out for sure using the techniques we've described with Linear Regression. 





## Logistic Regression 

## Decision Tree

## SVM

## Naive Bayes

## KNN

## K-Means

## Random Forest

## Dimensionality Reduction Algorithms

## Gradient Boost and Adaboost
