# Eigenvectos, Eigen Values
+ multiplying matrices repeatedly leads to the product approaching a number
+ for the inverse matrix the number approached is something different

## Typical behavior
+ the vector will converge to a certain line
+ the inverse will converge to a different line
+ applying a matrix to one of these special values will give a multiple of the original matrix

## Definition
+ A**v** = λ**v** for some λ and **v** ≠ 0
+ **v** is the eigenvector, λ is the eigenvalue
+ given λ it is fairly easy to find **v**
+ otherwise this is an extremely complex computational problem

## Eigenvectors
+ they are not unique
+ any multiple of a vector is an eigenvector

### Null Space
+ all non zero vectors in null A are eigenvectors with λ=0

## Linear independence
+ Vectors with different eigenvalues are linearly independent

## Calculating eigenvalues / vectors
+ find the charecteristic equation
    + det(A - λI) = 0
    + for a 2 * 2 matrix there is a simple equation
        + λ^2 - trA * λ + det A = 0
            + tr A is the sum of the diagonal entries of the matrix
+ solve the charachteristic equation
+ the solutions are the eigenvalues
+ the eigenvetors are Nul(A - λI)
+ the matrix always has rows that are multiples of one another
+ this means that the Null Space can be easily computed by reversing the order of the elements in a row and changing the sign of one of them

## PDP^-1 Factorization
+ P is the matrix of the eigenvectors of A
+ D is the matrix of the eigenvalues of A along the diagonal in the same order that the eigenvectors are in P
+ P^-1 is the inverse of P
+ Result is A = PDP^-1
+ Allows for relatively easy computation of P^n
    + P^n = P D^n P^-1
    + since D is a diagonal matrix D^n is easily computed
+ This factorization is only possible if there exists a basis of eigenvectors
    + this can be a consequence of all roots of characteristic polynomial being distinct
