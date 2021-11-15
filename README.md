# MultipleLinearRegression
MLR is a statistical technique that uses several explanatory variables to predict the outcome of a response variable.

Multiple linear regression (MLR), also known simply as multiple regression, is a statistical technique that uses several explanatory variables to predict the outcome of a response variable. MLR is an extension of linear (OLS) regression that uses just one explanatory variable and is used extensively in econometrics and financial inference.

Simple linear regression is a function that allows an analyst or statistician to make predictions about one variable based on the information that is known about another variable. Linear regression can only be used when one has two continuous variables—an independent variable and a dependent variable. The independent variable is the parameter that is used to calculate the dependent variable or outcome. A multiple regression model extends to several explanatory variables. [Source](https://www.investopedia.com/terms/m/mlr.asp)

_“If we have one dependent feature and multiple independent features then basically call it a multiple linear regression.”_  [Source](https://www.analyticsvidhya.com/blog/2021/05/multiple-linear-regression-using-python-and-scikit-learn/)

### Hyperparameters

- fit_intercept: Whether to calculate the intercept for this model. If set to False, no intercept will be used in calculations (i.e. data is expected to be centered).
  - bool
  - default=True
- normalize: This parameter is ignored when fit_intercept is set to False. If True, the regressors X will be normalized before regression by subtracting the mean and dividing by the l2-norm. If you wish to standardize, please use StandardScaler before calling fit on an estimator with normalize=False.
  - bool
  - default=False
- copy_X: If True, X will be copied; else, it may be overwritten.
  -  bool
  -  default=True
- n_jobs: The number of jobs to use for the computation. This will only provide speedup in case of sufficiently large problems, that is if firstly n_targets > 1 and secondly X is sparse or if positive is set to True. None means 1 unless in a joblib.parallel_backend context. -1 means using all processors. See Glossary for more details.
  - int
  - default=None
- positive: When set to True, forces the coefficients to be positive. This option is only supported for dense arrays.
  - bool
  - default=False

[Source](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)

## Necessary Packages
```
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split, cross_val_score, cross_val_predict
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, r2_score
```

## Dataset: Advertising

Book: An Introduction to Statistical Learning 

Available on [this page](https://www.statlearning.com/resources-first-edition)

## Example

 - Dataset: Advertising.csv
 - Preprocessing: 
   - Fixing index problem
   - Cleaning - missing data
 - Evaluation Metric: RMSE
 - Validation: Rsquared Cross Validation

## Further

[Multiple Linear Regression Using Python and Scikit-learn](https://www.analyticsvidhya.com/blog/2021/05/multiple-linear-regression-using-python-and-scikit-learn/)

[Linear Regression: Implementation, Hyperparameters and their Optimizations](http://pavelbazin.com/post/linear-regression-hyperparameters/)
