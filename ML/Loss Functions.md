#### Loss function: a function that maps events or values of 1 or more variables onto a real number, representing some "cost" associated with the event. Optimzation seeks to minimize loss


## Classification Losses:
Binary Cross-Entropy Loss (BCE) / Log Loss:
* calculates the logarithmic of the magnitude change, as opposed to squared loss which is the distance of the predicted to the truth.
* Binary:
	* $L = -\frac{1}{m} \sum_{i=1}^{m} \left( y_i \cdot \log (\hat{y_i}) + (1 - y_i) \cdot \log (1 - \hat{y_i}) \right)$ 
* Multiclass:
	* $L = -\frac{1}{m} \sum_{i=1}^{m} y_i \cdot \log (\hat{y_i})$
* BCE logits:
	* saves a step
	* BCE + sigmoid, takes in raw ouputs from detections
	* Less loss with precision loss of numerical values

Hinge Loss: [][]do later

## Regression losses:
Mean Square Error / L2 Loss
* average of squared differences between truth and predicted
* $\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} \left( Y_i - \hat{Y}_i \right)^2$
* penalizes the model for making large errors by squaring them,making the MSE cost function less robust to outliers
* you shouldn’t use it if the data is prone to many outliers

Mean Absolute Error / L1 Loss
* the average of absolute differences between the actual and the predicted value
* $\text{MAE} = \frac{\sum_{i=1}^{n} \left| y_i - x_i \right|}{n}$
* more robust to outliers compared to the MSE loss function
* you _should_ use it if the data is prone to many outliers.

Huber Loss / Smooth Mean Absolute Error
* combination of MSE and MAE, switching between by the choice of delta
* $L_{\delta}(y, f(x)) = \begin{cases} \frac{1}{2} (y - f(x))^2, & \text{for } |y - f(x)| \leq \delta, \\ \delta |y - f(x)| - \frac{1}{2} \delta^2, & \text{otherwise}. \end{cases}$
* effectively chosen to use MSE but have MAE for outliers
* Choice of delta is the choice of what you consider an outlier

Log-Cosh Loss
* logarithm of the hyperbolic cosine of the prediction error.
* $L(y, y^p) = \sum_{i=1}^{n} \log \left( \cosh(y_i^p - y_i) \right)$
* “Log(cosh(x)) is approximately equal to (x ** 2) / 2 for small x and to abs(x) - log(2) for large x. This means that ‘logcosh’ works mostly like the mean squared error, but will not be so strongly affected by the occasional wildly incorrect prediction.”

Quantile Loss
* for predicting quantiles
* $L_{\gamma}(y, y^p) = \sum_{i: y_i < y_i^p} (\gamma - 1) \cdot |y_i - y_i^p| + \sum_{i: y_i \geq y_i^p} \gamma \cdot |y_i - y_i^p|$


For Object Detection


Regularization:
* penalizes model complexity during training 
* Without it, in logistical models, the asymptotic nature of logistic regression would keep driving loss towards 0 in cases where the model has a large number of features.
* Strategies:
	* [[L_2 regularization]]
	* Early Stopping:
		* Limiting training epochs by some patience after a minimium loss is maintained, before it fully converges
		* Quick and easy, but not great way of regulariziting models, much better to L_2 regularization

[[Regularization rate (lambda)]]
[[Learning Rate]]


https://developers.google.com/machine-learning/crash-course/overfitting/model-complexity <- regularization 


https://builtin.com/machine-learning/common-loss-functions <- loss function
