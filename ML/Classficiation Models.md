ResNet:
* uses residual blocks, which are skip connections that allow the identity form a previous layer to be added on to layers after it, effectively outputing the identity + whatever the new layers output
* Solves problems like vanishing gradient and exploding gradient because the identity is always there