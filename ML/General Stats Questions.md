
##### "How describe common learning strategies"
* Supervised: model makes predictions and is given the correct answers to learn from and correct itself
* Unsupervised: model learns by developing relationships regarding the data itself, doesn't need to be taught what is correct
* Semi-supervised: some data is labelled
* Reinforcement: model is rewarded/punished for progress towards a goal based on previous actions 
##### "How would you train on unbalanced data?"

##### "How do you tell if a model is overfitting?"
* Overfitting: model learns too much from the training set, doesn't learn to properly generate relationships outside of it
* Signs:
	* Very high accuracy and loss on training set, much lower on validation and test
	* accuracy vs epoch curve tells us vs training and testing if the validation plateaus while the accuracy keeps on increasing, good indication
* Fixes:
	* regularization of data and inputs
	* simple models: less to memorize on
	* LASSO for penalization of the paramaters 
	* cross validation

##### "What Is ‘naive’ in the Naive Bayes Classifier?"
* classifier that assumes that the predictors are independent


##### "How Will You Know Which Machine Learning Algorithm to Choose for Your Classification Problem?"
* Concerned with accuracy or validity: test different algorithms and cross-validate
* train set is small: use models with low variance and high bias
* train set is large: use models with high variance and little bias

Bias: models are biased if the predicted value is far from the truth. Lower the better

Variance: amount the model will change when the model is trained on a different set of data. Overfitting is caused by high variance models learning on random noise rather than intended outputs 

###### What is the Trade-off Between Bias and Variance?
* bias-variance decomposition
* learning error comes from any algorithm adding bias, variance and irreducible error due to noise in the dataset
* Complex models have less bias, but more variance
* High bias and low variance = consistently bad
* Low bias and high variance = inconsistently good

Low variance models:
* linear regression, logistic regression, linear discriminate analysis
High variance models:
* []idk



