ResNet:
* uses residual blocks, which are skip connections that allow the identity form a previous layer to be added on to layers after it, effectively outputing the identity + whatever the new layers output
* Solves problems like vanishing gradient and exploding gradient because the identity is always there


InceptionV3 (compared to previous versions)
* Uses 3x1 and 1x3 convolutions instead of 3x3,  33% less params
* uses two 3x3 convolutions instead of 5x5, 28% less params
* uses two 7x1 and 1x7 convolutions instead of 7x7
* uses auxillary classifiers for training the layers, because the loss between the auxillary classifier can be added to the actual classifier to improve results and solve vanishing gradients

Xception:
* inceptionv3, but instead it has a bunch of 3x3 convolutions that are concatenated with each other after each one is passed through a 1x1 convolution.
* has skip connections of seperatable convolutions, all of the same dimensionality and activation

![[Pasted image 20250204101739.png]]

VGG16:
* very large, basic model with just convolutions, max pooling layers