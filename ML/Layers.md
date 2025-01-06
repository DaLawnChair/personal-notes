## Conv

## Pooling
2D filter over each channel of the feature map that summarizes the result

$(n_h - f + 1) / s \times (n_w - f + 1)/s \times n_c$
$$
\begin{itemize}
	\item[] n_h - height of feature map 
	\item[] n_w - width of feature map  
	\item[] n_c - number of channels in the feature map 
	\item[] f - size of filter 
	\item[] s - stride length 
\end{itemize}
$$



Pooling layers are used to **reduce the dimensions of the feature maps**. Thus, it reduces the number of parameters to learn and the amount of computation performed in the network.
### Max pooling
### Global pooling



## Activations
### Softmax
### Sigmoid

### Relu
### Leaky Relu