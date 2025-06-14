Automatic Differentiation
* Set of techniques to evaluate partial derivatives of a function
* Central tool for automatic and simultaneous computation of numerical values from arbitrarily complex functions and their derivatives without need of symbolic representation of the derivative
* Only function rule or an algorithm describing the function is required to perform this
* Neither symbolic or numeric
* In theory, it is exact, and in practice it is much faster than symbolic algorithms

General idea
* relies on the principle that every operation decomposes to a sequence of elementary arithmetic operations and functions
* Applies chain rule repeatedly on these operations, where partial derivaties are computed automatically, with high precision, and with a small overhead over the original function
* Has the same accuracy of symbolic, but does not yield an expression

How is it performed?
* Forward mode:
	* We can decompose the function as a sequence of subfunctions
	* Given an input vector for a function f, we can calculate the forward pass of the vector by evaluating the function for each subfunction (primal) and the primal's derivative (tangents), which is trivally solvable
	* In general, the forward pass can be expressed for $f: R^n \rightarrow R^m$ which yields a Jacobian mxn sized matrix of function f, where rows are every entry (i,j) represents the partial with respect to the ith function and the jth variable
	* Ideal for when n<<m, such as when you have few inputs, but many outputs
	* This yields the following formulation 
	* ![[Pasted image 20250429184103.png]]
	* 
* Reverse mode:
	* How it is done:
		* perform a forward pass of the function tree, but instead of computing derivatives, we store the dependencies of the expression tree in memory 
		* After completiton of the forward pass, calculate the partial derivative with respect to the intermediate variables before it
		* At a point, we can calculate the derivative with respect to a given variable by summing the contributions of every subfunction before it
		* ![[Pasted image 20250429190203.png]]
	* You only need to calculate the reverse pass once in order to get partial derivatives for every subfunction!
	* Backpropagation is just a special case of reverse mode, where the adjoints have activations and weights + biases associated with it
	* Ideal for when m<<n, such as when you have a cnn
* Reverse-on-forward:
	* Goal is to compute the Hessian Vector function $H_fv$ for $f:R^n \rightarrow R$
		* We can compute the product without explicitly computing the Hessian matrix!
		* Useful for computing 2nd order partial derivatives of a function
	* take the forward mode to compute gradient vector $\nabla f \cdot v (set x=v)$
	* Differentiate with the reverse mode to compute $\nabla^2 f \cdot v = H_fv$
* Time complexity: 
	* Forward: n\*c\*ops(f)
	* Reverse: m\*c\*ops(f)
	* where c<6, typically c=2,3 and ops(f) is the # of operations performed by f
* Space complexity:
	* Forward: O(1)
	* Reverse: O(ops(f))
		* Can be optimized further to only store the necessary values, and duplicates are just recalculated (called rematerialization/checkpoints)
	


What methods are used to compute it?
* Operator Overloarded:
	* Generate the primative and the tangental value, can be thought of as 
	```python
	class Variable:
		def __init__(self,val,dot=0):
			self.val = val
			self.dot = dot
		def __add__(self,other):
			res = Variable(self.val+other.val, self.dot+other.dot)
			return res 
		#...
	```
* Source code transformation ()()
Other methods:
* Manual Differentation
	* Finding the derivative of even given function
	* Tedious when you have many many terms to calculate partial deriviatives of various degrees for
* Numerical:
	* Approximating the slope with a sufficiently small h in $$f: R^n \rightarrow R, \frac{\partial f}{\partial x_i} = \frac{f(x+he_i)-f(x)}{h}$$ where $e_i$ is the axis.  
	* Problems: 
		* O(n) operations to calculate, which isn't good when you have millions of parameters
		* rounding accuracy, too small of a chosen h value will lead to error terms affected by the precision of floating point arithmetic
* Symbolic
	* Automatic version of manual differentiation using the derivative rules
	* Problems:
		* Expression swell:
			* ie product rule with generate at least 2 more terms to now evaluate
			* Commonly the soft ReLU (aka softplus) ($log(1+e^{wx+b})$) yields large terms
		* Required closed form expression, cannot use control flow graphs that includes loops, recursion, or conditionals

References:
https://www.youtube.com/watch?v=wG_nF1awSSY
* Differentation methods, and rundown of automatic differentation