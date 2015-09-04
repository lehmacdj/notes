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
+ if you solve the system:
    + the solution set is a span of the number of variables equal to the span of the number of free variables
    + The solutions are not unique: there are many solutions
    + See page 6 of red to read solutions

##Non-homogenous systems
+ A*x* = *b*
+ let *x0* be a solution
+ any solution is of the form:
    + *x* = *x0* + *v*
    + where *v* is a generic solution of the homogenous solution
    + i.e. 2x + 3y = 5
    + [x\y] = [1\1] + λ[-3/2\1]

##Applications

###Balancing Chemical equations
+ create an equation:
```
aCH4 + bO2 -> cC02 + dH20

write a system of equations
a = c } for C
4a = 2d } for H
2b = 2c + d } for O

turn it into a matrix
[1, 0, -1, 0\4, 0, 0, -2\0, 2, -2, -1]

row reduce it
[1, 0, 0, -1/2\0,1,0,-1\0,0,1,-1/4]

you have one free variable
[a\b\c\d] = λ[1/2\1\1/2\1]
to solve additional conditions we take: λ = 2
so:
a = 1
b = 2
c = 1
d = 2

then substitute back into the chemical equation
CH4 + 2O2 -> CO2 + 2H20

tada!
```

