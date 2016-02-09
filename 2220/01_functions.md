# Functions Sec 2.1
+ A function F from R^n to R^m is a rule that assigns each X in D to a *unique*
  point F(X) where each element of F(X) is determined by f_n(x_n) for functions 
  x1, x2, x3, etc + effectively this function breaks up into several functions 
  on the real numbers 

## constant functions
+ ie F(x1, x2, x3) -> (2, 4)
+ We don't graph we map because this is easier to visualize

## linear functions
+ Def: L is linear if for any X and Y in R^n and a element of R:
    1. L(X+Y) = L(X) + L(Y)
    2. L(aX) = aL(X)
+ equivalently: L(aX + bY) = aL(X) + bL(Y)
+ additionally: 
    + it can be represented by a matrix

#### Question: Are Constant Functions Linear
+ No
+ Except L(X) = **0**

+ Linear functions f(x) = mx + b are not linear
    + this kind of a function is considered an affine function
    + linear functions are only f(x) = mx or F(X) = AX
+ smaller functions are also linear li(aX + bY) = ali(X) + bli(Y)
    + there is a vector C such that li(X) = C . X for all X element of R^n
+ L(X) = (l1(X), l2(X), ..., lm(X)) = (C1 . X, C2 . X, ..., Cm . X)
    + therefore it follows that every linear function can be represented by a
      vector times
    + L(X) = MX
    + ||L(X)|| = ||MX||
    + This is the Generalized C-S theorem
        + ||MX|| <= ||M|| ||X||
            + ||C|| is the norm of the sum of the squares of all of the elements
              of the matrix
