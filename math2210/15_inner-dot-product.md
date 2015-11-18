# Inner and Dot Product
## Dot product
+ dot product = sum of xi * yi for 1..n of two column vectors in R^n
+ is equivalent to x^Ty 
+ x . x = square of the distance from O to x
    + is also equal to ||x||^2
+ || y - x || = sqrt((y - x) . (y - x))
+ || x + y || ≤ || x || + || y ||
+ -||x|| * ||y|| ≤ x . y ≤ ||x|| * ||y||
    + x . y = ||x|| * ||y|| * cos(theta)
    + correlation - they match closely
+ if x . y = 0 x and y are orthogonal

## Orthonormal Bases
+ if for u1..uk, ui . uj = 0 and ui=ui the basis is orthonormal
+ if U^T U = Ik then u1..uk is orthonormal

## Orthonormal Transformations
+ if U has orthonormal columns: (Ux) . (Uy) = x . y
+ The transformation preserves:
    + length
    + orthonagality
+ The orthogonal projection is UU^T

## Gram Schmidt Process
+ a way to get an orthonormal basis
+ contruction process
+ Arbitrary basis v1..vk of W (subspace of R^n)
+ 2 main steps
    + orthogonal basis w1..wk
    + orthonormal basis
+ The process:
    + one vector at a time
    + w1 = v1
    + w2 = v2 - Cw1 and w1 . w2 = 0 then C = w1 . v2
    + w3 = v3 - C1w1 - C2w2 where C1 = v3 . w1 and C2 = v3 . w2

## QR Factorization
+ A = QR
+ A has lin ind. cols
+ Q is a m * n matrix with orthonormal columns
    + obain through graham schmidt process
+ R is a upper triagonal matrix with positive entries on the diagonal

