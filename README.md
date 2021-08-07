## ACTUARIAL LOSS PREDICTION

Here we predict the loss which is the utimate claims during an accident by applying several models such as lasso regression , Xgboost and light gradient boost.
This is part of a competition conducted by IFOA as part of the actuarial Data science domain.

## STEPS INVOLVED

1) Firstly we import several packages and take a peek into our data.

2) We do an exploratory data analysis in which we look at the behaviour of several variables and adjust the variables-

  a) First we adjust the claim size by converting it into a log value . We see that the claims graph follows a distribution similar to pareto or exponential distribution and     therefore find the log value . 

  b) We see that the missing data is only of marital status and therefore make adjustments to it to remove the missing values.

  c) We change the date valiable by changing it to month , day , year and time difference . We also explore the behaviour of other variables.

  d) We conduct label encoding in which we change the categorical variables into numerical variables. 
  
3) We see the most important factors using extra tree regressor , perform min-max scalar by subtracting by minimum and dividing by difference of maximum and minimum and divide the data into training and test data.

4) We try out Lasso regression which removes paraeters of less significance , light gradient boost and xgboost and use hyperparameter tuning to make a model and test using mean squared errors .

5) Finally we see that light gradient boost techniques leads to predicting the best output although xgboost and lasso regression also seem quite accurate.
