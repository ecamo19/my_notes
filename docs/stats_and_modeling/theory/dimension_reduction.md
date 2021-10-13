# Dimension Reduction Methods

When n << p and/or there is collinearity the variance will increase so OLS will not perform well, so other methods are need to overcome this. 

These methods control variance by transforming the predictors and then fit a least squares model using these transformed variables. With these methods overfitting is avoid by using a less flexible approach.

If the correlation among predictors is high, then the ordinary least squares solution for multiple linear regression will have high variability and will become unstable OR  if n << p  least squares will be unable to ﬁnd a unique set of regression coeﬃcients that minimize the SSE


## PCR
Does not perform feature selection

Sometimes dimension reduction via PCA does not necessarily produce new predictors that explain the response.

+ The scores indicates if a value is below or above average. For example if the score < 0 in a PCA with two variables, then this indicates a city with below-average population size and below average ad spending. 

## PLS
Kuhn: We recommend using PLS when there are correlated predictors and a linear regression-type solution is desired


PLS identifies new features in a supervised way by making use of the response Y in order to identify new features that not only approximate the old features well, but also that are related to the response.

PLS ﬁnds linear combinations of the predictors

## What Goes Wrong in High Dimensions?

Cp, AIC, and BIC approaches are not appropriate in the high-dimensional setting, because estimating $\sigma^2$ is problematic.


## PCR vrs PLS
Since the directions in PLS are obtained by integrating the response variable, they explain more variation in Y than the principal components regression do. PLS also gives similar loadings to correlated variables, but variables that are correlated with the Y receive more weights compared with PCR. 