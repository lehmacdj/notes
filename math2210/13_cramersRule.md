# Cramer's Rule
+ For an equation A**x** = b
+ the solution is xi = det Ai(b) / det A
    + where Ai(b) is the replacement of the ith column of A with b
+ very difficult computationally
    + really only useful when you want to avoid division
    + such as with variables for functions
+ A^-1ij = det(Ai(ej))/detA = -1^(i + j) detAji / det A

## Area of Vectors in R^2
+ A = | det[v1 v2] | 

## Area of Triangle
+ A = 1/2 det[**1**, **x**, **y**]
+ The same works in greater dimensions
+ det T Area(S) = Area(T(S))
    + Corrolary: if A and B are matrixices of T in different basises tehn detA = detB

