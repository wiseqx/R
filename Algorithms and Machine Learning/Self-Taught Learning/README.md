# Self-Taught Learning

This file is going to implement self-taught learning for Neural Network using the Autoencoder.

I. Load data
sets and required libraries (e.g., H2O).

II. Train an autoencoder with only one hidden layer and change
the number of its neurons to: 20, 40, 60, 80, .., 500 (i.e. from 20 to 500 with a step
size of 20).

III. For each model in Step II, calculate and record the reconstruction error which is
simply the average (over all data points while the model is fixed) of Euclidian
distances between the input and output of the autoencoder (
“h2o.anomaly()” function can be used). Plot these values where the x-axis is the number of units
in the middle layer and the y-axis is the reconstruction error. 

IV. Use the 3-layer NN or “h2o.deeplearning” function (make sure you
set “ autoencoder = FALSE”) to build a model with 100 units in the hidden layer using
all the original attributes from the training set. Then, calculate and record the test
error.

V. Build augmented self-taught networks using the models learnt in Step II. For each
model:
A. Add the output of the middle layer as extra features to the original feature set,
B. Train a 3-layer NN (similar to Step IV) using all features (original + extra).
Then calculate and record the test error.

VI. Plot the error rates for the 3-layer neural networks from Step IV and V while the
x-axis is the number of features and y-axis is the classification error.

VII. Report the optimum number(s) of units in the middle layer of the autoencoder in
terms of the reconstruction and misclassification errors.

VIII. Comparing the plot from Step III and VI, explain any relation between
the reconstruction error and misclassification error.
