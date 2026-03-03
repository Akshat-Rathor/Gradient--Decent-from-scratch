Gradient Descent from Scratch 📉
A Python implementation of the Gradient Descent algorithm built from scratch, without relying on any ML library for the core learning logic. 
This project was built as part of my 100 Days of Machine Learning journey, inspired and guided by CampusX.

What is Gradient Descent?
Gradient Descent is an optimization algorithm used to minimize a cost function by iteratively updating model parameters in the direction of 
the steepest descent (negative gradient).In the context of Linear Regression, we try to find the best values of:

m (slope)
b (intercept)

such that the Mean Squared Error (MSE) is minimized:
MSE = (1/n) * Σ(Y - (mX + b))²
At each iteration, the parameters are updated using:
m = m - lr * dMSE/dm
b = b - lr * dMSE/db
Where:

lr = learning rate (controls step size)
The gradients are:

dMSE/db = (-2/n) * Σ(Y - mX - b)
dMSE/dm = (-2/n) * Σ((Y - mX - b) * X)


🛠 Implementation Details
Built using NumPy only
No use of sklearn for training logic Supports:
Custom learning rate
Custom number of epochs

Includes:
Model training (fit)
Prediction (predict)
Performance comparison with sklearn
