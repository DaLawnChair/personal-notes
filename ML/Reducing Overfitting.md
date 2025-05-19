Ranked:
* Dropout
	* Easiest to implement
* Batch normalization
	* Faster convergence
* Weight decay
* [[L_1 Regularization]] and [[L_2 regularization]]
* Early Stopping
	* Finkicky to tune patience and doesn't guarentee it has finished training fully when it has passed the threshold
* Data augmentation
	* Easy to do, but the model most be doing well already in terms of loss

Regularization:
* penalizes model complexity during training 
* Without it, in logistical models, the asymptotic nature of logistic regression would keep driving loss towards 0 in cases where the model has a large number of features.
* Strategies:
	* [[L_2 regularization]]
	* Early Stopping:
		* Limiting training epochs by some patience after a minimium loss is maintained, before it fully converges
		* Quick and easy, but not great way of regulariziting models, much better to L_2 regularization
		* Doesn't guarentee it has finished training fully when it has passed the threshold
		* Not guarenteed to stop the model from overfitting, needs to play around with patience and threshold
		* 
	
https://developers.google.com/machine-learning/crash-course/overfitting/model-complexity <- regularization 


Dropout(p)
* sandwiched between two layers, it will send each of the input layer's output to the output layer to 0 with probabilitity p
* Forces the model to adapt to noisier input, bettter generalzing
* Most commonly used between layers in the Fully Connected (FC) Layer
* Do not overuse at it can drastically affect the learning
* Generally 50-80% is a good parameter, increase as the model gets larger

https://machinelearningmastery.com/dropout-for-regularizing-deep-neural-networks/#:~:text=Dropout%20Rate,-The%20default%20interpretation&text=A%20good%20value%20for%20dropout,rate%2C%20such%20as%20of%200.8.


Batch Normalization
dependent on batch size
**NOTE, batch norm and dropout do not perform nicely with each other https://arxiv.org/abs/1801.05134**


Data augmentation:
* augments data to get more of them
* Make sure the augmentation preseverse data to its domain, ie do not augment rotation-reliant classes like for OCR tasks and medical images.
* **Only do so when training is showing near 0 loss**