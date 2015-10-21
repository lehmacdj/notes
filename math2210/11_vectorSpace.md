#Vector spaces
+ A set with 2 operations
+ addition
+ scalar multiplication
+ both of these must be closed

##Axioms
+ v + u = u + v
+ v + (u + w) = (v + u) + w
+ ...
+ the same axioms as before

## Example: 
+ R^n is a vector space
+ n * m matrix M(R)
+ vectors in 3d
+ Space of all smooth functions R -> R with pointwise operations
    + an infinite dim. vectorspace

## Linear transformations
+ a transformation is linear if it maintains the linear properties

## Kernel of a function
+ a set of functions that makes up a vector space
+ the null space of the transformation
+ { all v in T | T(v) = 0 }

## Range of a function / IMage
+ The possible results of a function
+ Column space of T
+ { for all w in v | there exists v in T and T(v) = w }

## Diferential operator
+ Null space of D is finite dimensional given any differentiable operator, and the dim is the order of D

## Basis of a vector space
+ spanning set which is linearly independent

### Pn - all polynomials of degree ≤ 2
+ Pn has a basis 1, x^1, x^2, ..., x^n
+ P2 also has the basis:
    + f1 = 1/2 x(x-1)
    + f2 = 1/2 x(x+1)
    + f3 = 1 - x^2
+ vectors can be formed to represent the coefficient of x^0..x^n these can represent the possible polynoimials
+ These different basises are very different to solve for, one involves solving a system but gives a solution that can easily convert lots of things
+ The other is faster for individual things but lags for large n of vectors to convert

##Dimension of vector spaces
+ The number of elements in a basis
+ Th: if V has basis B = {v1..vn} then any n+1 vectors {w1..wn+1} are linearly dependent
+ if W is a subspace of V then dimW ≤ dimV

## Rank
+ Rank V = dim Ker T + dim Im T
+ Rank T = dim Im T

## Maximum rank
+ rank T˚S ≤ min{rank T, rank S}

## Determinants are preserved
+ when a linear transformation is applied determinants are preserved
