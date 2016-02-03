# Continuity
1. Definitions
2. Some important concepts about sets / points
    + open ball
    + interior point
    + open set
    + boundary point
    + boundary
    + closed set
    + bounded set
3. important theorems - about closed sets and continuity

## Squaring
+ a = .010011000111000011110000011111...
+ a^2 = ?

## Definition
+ let F: D ⊂ R^n -> R^m. F is continuous at A ∈ D means: given any tolerance for
  error ε > 0 there is a precision δ > 0 so that if ||X - A|| < δ then
  ||F(X) - F(A)|| < ε

## Implications
+ size of mistake depends on the size of b and ε
    + for a very small a epsilon must be even smaller to get the desired
      precission
    + on a closed interval it is possible to get the correct level of accuracy
      δ based on the size of the values in the interval [-C, C]

## Uniform continuity
+ Important in computing in order to get a god level of precision for the
  specified task
+ one wants the right level for the entire domain of the function

## Intervals for functions of R^n
+  Let D be a set in R^n
+ Open ball in R^n centered at A of radius r > 0 is all the points X in R^n
   where ||X-A|| < r
+ A is an interior point of set D if there is an open ball of some radius r,
   centered at A contained in D
+ A point is boundary point if no matter what ball is drawn there are some
   things inside and outside the set
+ D is an open set if every point in D is an interior point
