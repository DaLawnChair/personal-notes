* Fundamentally how these machine learning frameworks are able to execute model inferencing and training.
* The goals of these are to implement a version of [[()()Automatic Differentiation (AD)]] in order to compute partial derivatives for the graph
* works by constructing graphs containing control flow and data structures to handle and process data
* Domains of interest: deep learning, physics engines, robotics, electronics, ray tracing, image processing, probabilistic programming
* Represented in two groups:
	* Static, compiled graphs:
		* Pros:
			* Good for compiler optimization
			* Scalability to larger systems
		* Cons: 
			* limits interactivity of systems 
			* types of models created (ie no loops or recusion) 
			* Hard to reason
		* Used by Tensorflow 1, Theano, and MXNet
	* Operator Overloarded, dynamic graphs
		* Pros: 
			* dynamic, ineractive nature for more verbosely described models
		* Cons:
			* interpreter overhead in execution
			* poorer scalability
			* reduced benefits from compiler optimzation
		* Used by Pytorch, Tensorflow 2, Numpy, and Pyaudi
			* Pytorch can be compiled using [[TorchDynamo]]
https://www.geeksforgeeks.org/dynamic-vs-static-computational-graphs-pytorch-and-tensorflow/ ()()



References:
https://en.wikipedia.org/wiki/Differentiable_programming








