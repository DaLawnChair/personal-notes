

Vector

std::vector<type> is a dynamically sized arrays for c++.


Vectors has slightly more overhead than static arrays as they allow for dynamic resizing. It can handle resizing automatically when the allocated memory is exhausted and it must reallocate more memory.

For most cases, elements are stored contigiously. Thus the elements can be accessed via offsets from the start. And so pointers to the start of the vector may work for iteration and
a pointer to the element of a vector may be passed to any function that expects a pointer to an element of an array.



constexprs:
Member functions of std::vector are constexpr, and so you can create and use std::vector objects in the evaluation of constant expressions. 
But they are not generally constexpr, as any dynamically allocated storage must be released in the same evaluation of constant expression.

Template Parameters:
    T must be: 
    * CopyAssignable: (t=v)
    * CopyConstructible: (T u = v and T(v))
    * Erasable (based on the operations performed on container): can be destroyed by a given Allocator


Allocator: used to acquire/release memory and to construct/destroy elements in memory. Not defined behaviour if Allocator::value_type is not the same as T.


**Special case: vector<bool>:**
This is specifically for bitsets



# Member Types:
* value_type T 
* allocator_type Allocator
* size_type Unsigned integer (usually std::size_t)
* difference_type signed integer (usually std::ptrdiff_t)
* reference value_type& 
* const_reference const value_type&
* pointer: std::allocator_traits<Allocator>::pointer (>c++11)
* const_pointer: std::allocator_traits<Allocator>::const_pointer (>c++11)
* iterator: LegacyRandomAccessIterator, contiguous_iterator, and ConstexprIterator to value_type (>=C++20)
* const_iterator: LegacyRandomAccessIterator, contiguous_iterator, and ConstexprIterator to const value_type (>=C++20)
* reverse_iterator: std::reverse_iterator<iterator>
* const_reverse_iterator: std::reverse_iterator<const_iterator>



# Member Functions:
* (constructor)
* (destructor)
* operator= (copying elements from any vector)
* assign (copying elements from any container )
* assign_range (basically assign but without needing to do `dest.assign(container.cbegin(), container.cend())` and can instead do `dest.assign_range(container)`, C++23)
* get_allocator



# Different types of initializations
```c++
#include <vector>
using namespace std;

int main(){
    vector<int> v1(100,2); // 100 elements, all are 2
    vector<int> v1{100,2}; // elements are 100 and 2 



}

```
# Basic usage
```c++

#include <vector>

int main(){
    std::vector<int> v = {8, 4, 5, 9}; // construction
    
}

```



# std::views

std::views::filter(func)
* filters through the given data with func

std::views::transform(func)
* transforms the data with func


# references:
https://www.youtube.com/watch?v=Xx-NcqmveDc 
* very good overview on how a simple code of just having a making an array, then setting the array's value to another array can be optimized
	* Use const if you are working with the original and do not need to copy every element
	* call vector.reserve() if possible to the desired compacity as the default will grow from its default compacity
	* do not use vector.pushback(Data(args)) where data is an object. This will call the constructor of it and can lead to too many calls. Should use vector.emplace_back(args_for_data) in order to construct in place
		* Not that vector.emplace_back(Data(args)) is just as bad, so avoid if possible
	* Note that alternatively you can do moves instead, as long as the Data structure has a move function. This isn't necessarily always better though and can still lead to too many instance for your needs
*

https://en.cppreference.com/w/cpp/container/vector.html
https://en.cppreference.com/w/cpp/container/vector_bool.html

