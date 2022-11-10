# matrix_vector_for_python
Just my own implementation of matrices, vectors, polynomials and rational numbers  done just for fun.

The demo code in demo_matrix.py shows how to use the trivial library. Given the fact that libraries like pandas, numpy exist, it is obviously unnecessary to come up with a matrix and vector implementation. Nonetheless, I did it for the fun of experimentation.

Note: Rational cannot be used as a dtype for Matrices as this does not make a lot of sense. You may use the Rational.float() conversion to bridge the gap.


Pros and Cons

Pros:

+ minimalistic library that constrains itself to essential functionality
+ call by value: only the setters __setitem__ manipulate an object directly. All other functionality tries to stick to a functional approach
+ small code size
+ easy to use (see the implementation of QR decomposition as an example)
+ pure Python

Cons:

+ requires more memory that the memory-efficient numpy arrays
+ uses efficient algorithms whenever possible, but is not optimized for runtime efficiency
+ does not provide any means for multithreading

Usage: see demo code
