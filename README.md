# Logistic-Reg-Predict-Customer-Churn

Design outline

Preprocess the data:
a. Feature scaling: Instantiate an object of the FeatureScaler class to scale the input features to have zero mean and unit variance, using the fit_transform() method of the FeatureScaler class.
b. Feature selection: Instantiate an object of the FeatureSelector class to select the most important features using the fit_transform() method of the FeatureSelector class.
c. Split the data into training and test sets using a function such as train_test_split() from the scikit-learn library.

Train the model:
a. Instantiate an object of the LogisticRegression class with the desired hyperparameters such as learning rate and number of iterations.
b. Train the model on the training set using the fit() method of the LogisticRegression class.

Evaluate the model:
a. Predict the labels of the test set using the predict() method of the LogisticRegression class.
b. Compute various metrics to evaluate the model's performance using the BinaryClassificationMetrics class, such as confusion matrix, accuracy, precision, recall, and F1-score.

Fine-tune the model:
a. To prevent overfitting, use regularization by instantiating an object of the Regularizer class and passing it to the LogisticRegression class's fit() method.
b. To improve convergence, try different optimization algorithms such as GradientDescent, StochasticGradientDescent, and AdamOptimizer, by instantiating an object of each class and passing it to the LogisticRegression class's fit() method.