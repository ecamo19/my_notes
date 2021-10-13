# Model selection

## Best Subset Selection

Fit a separate least squares regression for each possible combination of $p$ predictors. That is, fit all possible combinations and evaluate all the possibilities. 

The problem with this is that we have to evaluate $2^p$ models which is computationally expensive. 

## Forward Stepwise Selection

This method starts with a null model with no predictors, then add a predictor, evaluate the model and repeats.

Forward selection can be applied when n < p but only to $M_0$ ..... $M_{n - 1}$  since  n >= p will not yield a unique solution.
 
## Backward Stepwise Selection
This method begins with the full least squares model containing all p predictors. This works when n > p


## Choosing the Optimal Model Cp , AIC, BIC, and Adjusted R^2

+ Cp: Add a 2d$\sigma^2$ penalty that increases as the number of predictor increase. Cp ~ AIC

+ BIC: Usually BIC chooses a model with less predictors that the one chosen by Cp 

## One-standard-error rule. 

We first calculate the standard error of the estimated test MSE for each model size, and then select the smallest model for which the estimated test error is within one standard error of the lowest point on the curve.


## Do not use R^2 or RSS for selecting a model

The training error will decrease as more variables are included in the model, but the test error may not. Therefore, training set RSS and training set R^2  cannot be used to select from among a set of models with diﬀerent numbers of variables. $R^2$ increases with the number of predictors while RSS decrease.

