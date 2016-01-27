#Complexity

##Basic steps
+ input / output scalar value
+ access value of scalar variable array element or object field
+ assign to variable
+ do one arithmetic or logical operation
+ method call
    + not counting the execution of the body or argument parsing
+ if statement
    + number of things in branch that is executed
+ loop
    + number of things in loop times number of times executed
+ method
    + total of things in the method body

## Big O notiation
+ runtime complexity

###Goals
1. Distinguish among cases for large n, not small n
2. Distinguish amoung important cases, such as:
    + n * n basic operations
    + n basic operations
    + log n basic operations
    + 5 basic operations
3. don't distinguish between trivially similar cases. ie:
    + n and n + 2
    + n^2 and n^2/2
    + n^2 and n^2 + n

###Definition
+ f(n) is O(g(n)) if theree exist constants c and N such that for all n ≥ N, f(n) ≤ c * g(n)

###Properties
+ Only the term that grows most rapidly matters
+ O(n^2) is also O(n^3), etc.

###Problem size
+ using O(n) one can determine how large of an n one can use for a certain amount of time

###Worst and Expected Case
####Worst case
+ how much time is need for the worst possible input of size n

####Expected case
+ how much time is needed for the average input of size n
