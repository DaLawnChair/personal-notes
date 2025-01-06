## More data:
Scower more data 
Can also use data augmentation on the images themselves
Could also use image generation tools too.
* [Dreambooth - synthethic text-to-image generation given 3-5 images](https://dreambooth.github.io/)
	* Not sure what I'd change to the images though other than 'make light green, not red' or 'make arrow green and bulb red'
* 
## Feature selection
Select features that minimize variance between all pieces of data across the dataset. 
* If variance is high, drop some features

Too many features can overfit the model to the training data.

Feature selection methods:
* Random Forest
* XGBoost
* Dimensionality reduction
	* PCA

## Hyperamater Tuning
Tune specific parameters until the to find the optimal choice for each parameter given the range of values

## Ensemble model
Take results for multiple number of models of different architectures and training, then do a voting to select the concensus classification.
## Outlier Removal
Remove outliers from the dataset
* I worry because images of uncommon scenarios could technically an outlier given a small enough sample. However this worry goes away with more data points 

## Regulization techniques
Reduces complexity of models by reducing the amount the weights and/or biases change as model trains.

* Batch normalization: Normalizes inputs of each layer to reduce covariance shift and improve learning rate
* L1 and L2: add penalty term to loss function based on magnitude of weights