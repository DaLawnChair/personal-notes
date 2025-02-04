Sigmoid/ Logistic
$f(x) = \frac{1}{1+e^{-x}}$
* Usually used as the last layer for the binary classificaiton

softmax:
$S(y_i) = \frac{e^{y_i}}{ \sum e^{y_i}}$
* used as the last layer for multiclass classification
* converts the input into probabilities for each of the classes

TanH - Hyperbolic Tangent
$f(x) = \frac{2}{1+e^{-2x}} -1$
* used in hidden layers
* scaled and shifted sigmoid function between \[-1,1\]

ReLU - Rectified Linear Activation
$f(x) = max(0,x)$
* used in hidden layers
* Generally used if you don't know what activation function to use
* **dying relu problem**: after training, the output of the activation can always be 0, thus no more updates as neuron is dead

Leaky ReLU
$f(x) = x if x>=0, a\cdot x otherwise$
* small choice of a
* fixes dying relu problem
* use when weights do not update during training
