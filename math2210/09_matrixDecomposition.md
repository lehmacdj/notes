#Matrix Decomposition
+ Given a matrix A, we can express it as a product of "simple matrixes"

##LU decomposition
+ A = L U
    + } L is a square with ones on the digonal with 0 above diagonal
    + } U is in REF
+ finding L and U. Certain things cannot be done
    + no multiplying rows by another
    + no swapping rows
    + only modify lower row using upper row

##QR Decomposition (For squares)
+ A = Q R
    + } Q is orthoganal
    + } R is upper triangular

## Singular value decomposition
+ A = U D V
    + } U, V are orthoganal
    + } D is diagonal

## Spectral Decomposition
+ A = P D p^-1
    + useful for raising a matrix to a large power

##Subspaces
+ a subset of R^n
+ Conditions for a subspace
    + if **u**, **v** in U then **u** + **v** is also in U
    + the same is true for scalar multiplication
    + **0** is in U
+ A line could be a subspace of R^n
+ Column space of A
    + the span of the column vectors of A
    + all vectors **b** suchthat A**x** = **b** has a solution
+ Null subspace of R^n
    + all x ∈ R^n such A**x** = **0**
    + solutions of the homogenous system
