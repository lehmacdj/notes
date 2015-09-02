#Matrix equations
##Multiplication of a matrix and a vector
+ A * c = [1,2,3\7,5,2\1,0,-2] * [1\\-1\2] = 1 * [1\7\1] + -1 * [2\5\0] + 2 * [3\2\\-2] = [5\6\\-3]
+ A must have as many columns as c has rows
##Systems of linear equations
```
 x1 + x2 + x3 = 5
-x1 +2x2      = 7

=>
[1,1,1\-1,2,0][x1\x2\x3] = [5\7]
```
A*x* = *b*

You cannot divide by matrixes

##Properties of multiplying matrixes
1. A(*u* + *uv*) = A*u* + A*v*
2. A(a*u*) = a(A*u*)

***Theorem: The following are equivalent:***
1. A*x* = *b* has a solution for any vector *b*
2. every vector *b* is a linear combination of column vectors of A
3. span of columns of A is everything
4. REF of A has pivots in every row

+ Only the coefficient matrix is used for te above theorem

##Solving Matrix equations
A*x* = *b*

[A, *b*] 

=> row reduction

[A', *b*']

where:
+ A' = RREF of A
+ *b*' prime can be anything if we ahave a freedom to change *b*

+ has a solution unless there is a pivot in the last column
+ This can not happen if RREF of A has pivots in every column
+ You try to reverse the process in order to

##Homogenous System
+ A*x* = *0*
+ there is a solution
+ *x* = *0*
+ the zero solution or trivial solution
+ the question remains is there another solution

There is a solution for every free variable to this equation
