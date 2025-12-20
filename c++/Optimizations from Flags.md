


# Return Value Optimization and Copy Elision:

Even at O0, return value optimization is used to avoid copies from return values to the caller.

this prevents many, many copies when nested function calls, and avoids the necessary handling of pointers  to remove the redunancy. 

This operation is **blessed** by the compiler, and fundamentally changes the logic of the code.
For example, if you create and return a class that has a custom copy/move constructors, Return Value Optimization and Copy Elision may prevent those from being called.
* This is why you should always use your copy constructor to make copies, because it will never be as efficient when compiled by the optimizer for these copy calls
* this is why you should never use copy constructor for anything but copying, as it may not happen

When is this done:
* mainly when the constructed value is made for explicit use outside of the callee function. Ie the object is always made to be returned (or made and then some minor modification to it is done). This allows the constructed object to live inside of the caller function, instead of the callee, avoiding the copies
* construction of an object is sent as arguments into a function

When is it not done:
* when the constructed value is not determined at call time. (made up term by me). Ie there is logic that makes you chose between two constructed objects, so this requires it to live in the callee function

Resource:
https://www.youtube.com/watch?v=HNYOx-Vh_VA