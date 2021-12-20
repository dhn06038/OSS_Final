# Best model for image classification
The final project of OSS lecture is find the best model for image classification which has the highest accuracy.


## Framework to find the model
__First__, try several classifiers in scikit with default settings.

__Second__, choose some models which has high accuracy.

__Third__, change some hyperparameters until get highest accuracy.


## About codes
*Create a classification object*

__log_reg = sklearn.linear_model.LogisticRegression(C=100, random_state = 0, solver='liblinear')__

*Fit the object*

__log_reg.fit(X_train, y_train)__

*Predict the label of test data*

__y_pred =  log_reg.predict(X_test)__


## About hyperparameters
__random_state = 0__ *to avoid randomness issue.*

__solver='liblinear'__ *is good for small datasets.*

__c = 100__ *while changing the value of c, around 100 has the highest accuracy.*
