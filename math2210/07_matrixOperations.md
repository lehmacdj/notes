#Matrix operations
##Adding the linear transformations
+ Linear transformations can be added
    + T(x) = T'(v) + T"(v)
+ As a consequence matrixes can also be added

##Multiplying by numbers
+ (λT)(v) := λ(T(v)) = T(λv)

##Multiplying by matrixes
+ composition combines linear transformations
+ does one after another
+ the result will also be a linear transformation
+ AB <---> linear transformation R^k -> R^n
    + where A is m * k
    + and B is n * m
    + B is the matrix that is applied first
+ To multiply you multiply all of the column vectors of B by A and then put the result back into the original matrix
+ AB ≠ BA
    + often these do not even occupy the same space
    + or alternatively one may be undefined

##Properties of matrixes
1. A(B + C) = AB + AC
2. (A + B)C = AC + BC
3. λ(AB) = (λA)B = A(λB)
4. A(BC) = (AB)C
    + composition of functions is associative
5. There exists an identity matrix: InA = A = AIm
    + In is a matrix with ones on the matrix and zeroes everywhere else

##Transposition
A^T is A transposed (columns = rows and vice versa)

1. (A^T)^T = A
2. (A + B)^T = A^T + B^T
3. (λA)^T = λ(A^T)
4. (AB)^T = (B^T)(A^T)
    + requires work is not obvious

##Invertible matrixes
+ a matrix is invertible if there exists a matrix B such that for A (size n x m matrix) there exists a B such that AB = In and BA = Im
    + for square matrixes one of these implies the other
+ the inverse of a 2 x 2 matrix [a, b; c, d] = 1/(ad -bc) * [d, -b; -c, a]
    + it is only invertible iff ad -bc ≠ 0
        + ad - bc is the determinant of the matrix

###Computing inverses
+ the inverse of A is the row reduction of [A, In] to [Im, A^-1]

