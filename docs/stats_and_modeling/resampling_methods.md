# Resampling Methods

Resampling methods are used in the absence of very large designated test sets that can be used to directly estimate test error rates  

+ __Validation Set Approach__ 

Good when n is large. This method consist in dividing randomly the data set into Training and Test (Validation) data sets

Drawbacks:

1) High Variable, depends on the observations chosen 
2) Not all the data is included in training the model

+ __Leave-one-out cross validation (LOOCV)__

In this method a single pair observations ($x_1$,$y_1$) are left out for validation and the rest of the data is used for training being repeated n times

Drawbacks:

1) Expensive to implement (time consuming, the validation is done in n observations) 

+ __k-fold Cross Validation__

Randomly divide the whole data set in k groups of equal size. The first fold is used as validation set and the others are used as training sets. This procedure is repeated k times, each time, a different fold is treated as validation test. 

For example if k = 10 then the data set is divided into 10 folds, the first one will be used as validation set and then the statistical method (i.e. linear model) is fitted on each one of the other 9 folds. This is repeated until each one of the folds has being used as validation sets.  
