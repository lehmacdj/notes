#Inverses
+ a matrix is invertible if there exists a matrix B such that for A (size n x m matrix) there exists a B such that AB = In and BA = Im
    + for square matrixes one of these implies the other
+ the inverse of a 2 x 2 matrix [a, b; c, d] = 1/(ad -bc) * [d, -b; -c, a]
    + it is only invertible iff ad -bc ≠ 0
        + ad - bc is the determinant of the matrix

##Computing inverses
+ the inverse of A is the row reduction of [A, In] to [In, A^-1]
+ if RREF is not [In B] A is not invertible
+ works for any sized square matrix

##Properties of inverses
+ transposition and inversion are communtative
    + (A^T)^-1 = (A^-1)^T
+ (AB)^-1 = B^-1 A^-1
    + The order of the multiplication has to be inversed as well

##Why does this work?
+ every step of row reduction is just multiplication by a matrix
    1. multiply first row by λ an identity matrix with λ for one of the 1s
    2. swap rows: identity matrix with rows swapped
    3. add multiplied row: add multiple of matrix to first row of an identity matrix

+ if RREF of A is matrix B, there exists invertible n * n matrix C such that CA=B
+ if RREF of A is In => A s invertible and the inverse of A is C

##Why matrix inverses? 
+ if A is invertible then A**x** = **b** ahas a unique solution
    + **x** = A^-1**b**
    + Computing A^-1 takes longer than solving directly
    + only useful if many solutions in the form of A**x**i = **b**i are desired

##Inverse Matrix Theorem
***if A is an n*n matrix The Following are Equivalent***

1. A is invertible 
2. RREF of A is In 
3. A has n pivots
4. A**x** = **0** has ony the trivial solution
5. columns of A are linearly independent
6. the map **x** -> A**x** is 1 to 1
7. A**x** = **b** ahs solution for every **b**
8. columns of A span R^n
9. **x** -> A**x** is onto
0. there exists C | CA = In
1. there exists D | AD = In
2. A^T is invertible


