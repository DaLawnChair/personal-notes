 we want to `minimize(loss+model complexity)` ussually by `minimize(loss+ lambda*(model complexity) )`
* unknown exactly how to pick [][]do more research on this
* If lambda is high:
	* strengthens regularization, less overfitting
	* tends to generate histogram of model weights having
		* normal distribution of mean=0
* If lambda is low:
	* weakens regularization, encouraging overfitting
	* tends to generate histogram of model weights having flat distribution
