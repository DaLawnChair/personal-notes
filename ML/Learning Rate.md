numerical value telling gradient descent algorithm how strongly to adjust the weights and biases for each iteration
* If low, takes long to train 
* If high, may not converge

In general, we are performing:
	weights <- weights_old + learning_rate * delta gradient(weights_old)

When we are taking the batch size, we are averaging the delta over the weights
	weights <- weights_old + learning_rate * SUM_OF_BATCHES (delta gradient(weights_old) )
* Learning Rate should up with batch size
	* Think about the converse. Batch size scales down, we want learning rate to scale down too to match because otherwise we will learn too much from too small of a sample


