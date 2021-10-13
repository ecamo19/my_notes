# Bias-Variance trade-off

In a perfect scenario, a statistical method should achieve low variance and low bias 

+ __Bias__ 

Bias is defined as the error introduced by approximating a real life problem (which in nature could have complicated relationships) by a simple model

I associate bias as a model simplification. Like Fitting a linear model that follow a non-lineal trend 

+ __Variance__

How much a function $f$ would change if we estimated it using a different train set? 
High variance indicate that if we change a data point in the data the function $f$ will change. 

I associate variance with overfit. Models with high variance have high flexibility because those model adjust following each data point.

For example linear models have low variance but they could have high bias

Highly correlated predictors can lead to collinearity issues and this can greatly increase the model variance.

More complex models can have very high variance, which leads to over-ﬁtting. On the other hand, simple models tend not to over-ﬁt, but under-ﬁt if they are not ﬂexible enough to model the true relationship (thus high bias).