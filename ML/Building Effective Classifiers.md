# Explore premade solutions first

[[D] Is there a more systematic way of choosing the layers or how deep the architecture goes when creating a neural network?](https://www.reddit.com/r/MachineLearning/comments/1ckrzq6/d_is_there_a_more_systematic_way_of_choosing_the/?rdt=53852)
- If you're using Tabular data, try boosting first (something like XGBoost). It usually works better in this domain than neural nets and has less architecture choices.
- For vision, start with a pre-trained model. People used ImageNet pretraining but nowadays state of the art models are usually pretrained on ImageNet21K or in a self-supervised fashion (DinoV2, EVA, BeiT,...) on even larger datasets. With finetuning, you shouldn't run into overfitting issues and the larger should work better. So pick the largest one you can manage, or the smallest one that achieves the desired performance. Most people would nowadays use a vision transformer as architecture but a ConvNeXt can still be a reasonable choice. Don't try to come up with your own architecture, you won't get anything as good as existing models. If you don't want to fine-tune the entire model, you can also just use the backbone as fixed feature extractor or if you're using a ViT, use task adaptation like PEViT, Lora or Adapters.
- For language it's similar to the vision case. Start with a pre-trained LLM. They're usually even larger than vision models so there you typically only want to do LoRA finetuning instead of retraining the entire model during training.
- Typically you want to start off with a larger model that overfits to the data. 
	- Rational is that smaller models will perform bad until you add enough layers to overfit, but then you'd need to gridsearch and find other methods to cut down on the model, so might as well start large and just cut down.
- With tabular data, find the relationship between the data and your predicted column, the more correlation typically the easier it is to use a really small MLP model.
- With CNNs, pay most attention to Receptive fields - how much of the sequence each layer corresponds to
	- The reason why we add or remove layers is for achieving large/small receptive fields, not to satisfy a layer count


## More data:
Scower more data 
Can also use data augmentation on the images themselves
Could also use image generation tools too.
* [Dreambooth - synthethic text-to-image generation given 3-5 images](https://dreambooth.github.io/)
	* Not sure what I'd change to the images though other than 'make light green, not red' or 'make arrow green and bulb red'
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