# Extended automatic differentiation 
NOTE: This is an older version of the language. Soon I'll upload a newer version with much cleaner syntax 
that is a mix of python and c++ syntax. 

The idea of this language is that the fundamental data type is an extended dual number, which is a 
triplet of floats (f,f',f''). f is a function value, f' is the derivative, and f''
is the second derivative. Constants are just the special case (f,0,0). 

The algebra of the extended duals are defined so that first and second derivatives are carried around
and calculated as you go. As a result, arbitarily complex univariate functions can be maximized or minimized with
newtons method without needing to resort to symbolic differentiation or inaccurate numerical differentiation. 
