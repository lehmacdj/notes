#Matrixes
+ an array of numbers
+ m * n -- m rows, n columns
+ use capital letters to represent with a variable

##Linear equations
+ matrix can represent linear equations
+ easily convertable back and forth
+ the question remains how can one best simplify by row opperations?

## Single Matrix things
+ leading entry - left most non zero entry in each row
### Row echelon form
1. all zero rows are ath the bottom
2. leading entries at top rows are furthest to the left
3. all matrix entries below a leading entry are zero
### Reduced row echelon form
1. all conditions from row echelon form
2. all leading entries are 1
3. all entries above a leading entry are 0

***Theorem 1: Every Matrix can be reduced to a unique matrix in RREF***

### Row echelon form algorithm
+ a greedy algorithm

**only subtract from rows that are you aren't also changing at the same time fixed**

+pilot the entry of the matrix that you use to reduce the other rows

##Solving equations based on the matrix
+ typically it is enough to go to row echelon form rather than row reduced echelon form

### free variable
+ a variable for which there is no leading entry for its column
+ one can write the solutions in the form of the free variable(s)

### no solution
+ if there is a leading entry in the last column the equation has no solution
