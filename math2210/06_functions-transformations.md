# Functions / Transformations
##Functions
+ **image** -- the result of applying the fuction to an argumet
+ **restriction** -- limiting the size of the domain
+ we can think of matrixes as fuctions
+ a m * n matrix transforms a vector of dimension n to dimension m

###Domain
+ the set of possible arguments

###Co-Domaian
+ the entire set of possible solutions
+ range is the set of results that can actually be produced by the function
+ An argument produces a result that is always the same for the same function

### Onto
+ every point in the co-domain is an image of something

##The following are also equivalent -- ONTO
+ T is onto
+ T(x) = v has a solution for every **b**
+ RREF of the matrix has pivots in every row
+ The rows of the matrix are linearly independent

### 1 to 1
+ a fuction where different points in te domain have different images
+ to determine if a function is unique one has to determine if it has a unique solution
    + A**x** = **0** must have a unique solution

####The Following are equivalent -- 1 to 1
+ T is 1 to 1
+ T(v) = 0 has only a trivial solution
+ RREF of the matrix ovf T has pivots in every column
+ the columns of the matrix are linearly independent

       + if it is always true then the system is onto

## Transformations
+ a transformation is linear if the following is true
    1. T(u + v) = T(u) + T(v)
    2. T(λ * v) = λ * T(v)
+ this implies a few things
    1. T(**0**) = **0**
    2. if v1 ... vk are linear dependent, then T(v1) ... T(vk) are linear dependent
        + Corrolary: if T(v1) ... T(vk) are linear independent, then v1 ... vk are linear independent
        + The converse and inverse are not true
+ if a linear transformation R^m -> R^n is linear, then there exists a unique m * n matrix A | T(v) = Av for any v
+ a linear transformation is 1 to 1 if and only if the RREF of the matrix T has pivots in every column
+ a linear transformation is onto if and only if the RREF of the matrix has pivots in every row

### Constructing linear transformations
1. start with standard basis vectors
    + e1 = [1; 0; 0; ...; 0], e2 = [0; 1; 0; ...; 0], ... em = [0; 0; 0; ...; 1]
2. combine into a matrix
    + A = [T(e1), T(e2), ..., T(em)]

###Adding the linear transformations
+ Linear transformations can be added
    + T(x) = T'(v) + T"(v)
+ As a consequence matrixes can also be added

###Multiplying by numbers
+ (λT)(v) := λ(T(v)) = T(λv)

###Multiplying by matrixes
+ composition combines linear transformations
+ does one after another
+ the result will also be a linear transformation
+ AB <---> linear transformation R^k -> R^n
    + where A is m * k
    + and B is n * m 
    + B is the matrix that is applied first
+ To multiply you multiply all of the column vectors of B by A and then put the result back into the original matrix
