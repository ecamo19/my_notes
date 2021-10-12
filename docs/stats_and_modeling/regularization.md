# Shrinkage Methods

This methods work by controlling variance (less flexible methods) by shrinking coefs towards zero or exactly zero. With these methods overfitting is avoid by using a less flexible approach.

## Ridge Regression

Ridge Regression will include all p predictors in the final model. This method just shrink coefs towards zero.

$\lambda$ = Penalty term (l2), the larger the $\lambda$ is the smallest (towards zero) the coefs are.

Ridge regression’s advantage over least squares is rooted in the bias-variance trade-oﬀ. As $\lambda$ increases, the flexibility of the ridge regression fit decreases, leading to decreased variance but increased bias. At some point MSE will decrease.

Ridge regression works best in situations where the least squares estimates have high variance.

## Lasso Regression

The lasso shrinks the coefs to zero which can be use for variable selection

__Differences between lasso and ridge__

+ Penalty term
+ Lasso performs feature selection
+ Lasso will perform better in a scenario where a few p have a high coefs and the others are close to zero
+ Ridge will perform better when there are many predictors with with coefs of the same  ~size