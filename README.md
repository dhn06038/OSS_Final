# Best model for image classification
The final project of OSS lecture is find the best model for image classification which has the highest accuracy.

### Framework to find the model
First, try several classifiers in scikit with default settings.
Second, choose some models which has high accuracy.
Third, change some hyperparameters until get highest accuracy.

### About codes
*Create a classification object*
log_reg = sklearn.linear_model.LogisticRegression(C=100, random_state = 0, solver='liblinear')
*Fit the object*
log_reg.fit(X_train, y_train)
*Predict the label of test data*
y_pred =  log_reg.predict(X_test)

### About hyperparameters
random_state = 0 *to avoid randomness issue.*
solver='liblinear' *is good for small datasets.*
c = 100 *while changing the value of c, around 100 has the highest accuracy.*
