## Convolution

https://www.geeksforgeeks.org/what-are-convolution-layers/
https://github.com/google-research/tuning_playbook
https://keras.io/keras_tuner/api/tuners/bayesian/
## Pooling
2D filter over each channel of the feature map that summarizes the result

$(n_h - f + 1) / s \times (n_w - f + 1)/s \times n_c$  , where
$$
\begin{array}{ll}
n_h & \text{- height of feature map} \\
n_w & \text{- width of feature map} \\
n_c & \text{- number of channels in the feature map} \\
f & \text{- size of filter} \\
s & \text{- stride length}
\end{array}
$$

Pooling layers are used to **reduce the dimensions of the feature maps**. Thus, it reduces the number of parameters to learn and the amount of computation performed in the network.

Variations:
* Max pooling: take the max value from the given filter size convoluted with the input
	* Typically used in image data, because we want to distinguish defining features (ie edges)
* Average pooling: take the average from the given filter
	* smooths images
* Min pooling: take the minimum value from the given filter size convoluted with the input
	* Typically used in image data, because we want to distinguish defining features (ie edges) but for small values (see images below)

You can have global versions of each, which is just where the filter size is the same as the input size.

Source for images:
![[Pasted image 20250122064820.png]]
![[Pasted image 20250122064842.png]]


### Deconvolution Layer
* transposed convolution process that effectively upsamples data to a higher resolution

#### Recurrent Layer




Skip connections
Residual Blocks

Skip connections  (ie Resnet) https://chautuankien.medium.com/skip-connection-and-explanation-of-resnet-afabe792346c

