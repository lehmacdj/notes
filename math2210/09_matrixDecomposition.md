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

