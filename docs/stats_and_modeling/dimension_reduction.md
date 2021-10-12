# Dimension Reduction Methods

These methods control variance by transforming the predictors and then fit a least squares model using these transformed variables. With these methods overfitting is avoid by using a less flexible approach.

## PCR

Does not perform feature selection

+ The scores indicates if a value is below or above average. For example if the score < 0 in a PCA with two variables, then this indicates a city with below-average population size and below average ad spending. 

## PLS

PLS identifies new features in a supervised way by making use of the response Y in order to identify new features that not only approximate the old features well, but also that are related to the response.

## What Goes Wrong in High Dimensions?

Cp, AIC, and BIC approaches are not appropriate in the high-dimensional setting, because estimating $\sigma^2$ is problematic.


## PCR vrs PLS
Since the directions in PLS are obtained by integrating the response variable, they explain more variation in Y than the principal components do. PLS also gives similar loadings to correlated variables, but variables that are correlated with the Y receive more weights compared with PCR. 