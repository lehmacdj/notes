#Loops
##Expressions
+ Be concise
+ Be consistent
##Looping
+ Generalize a picture that is true before and after each iteration
+ initialization makes the picture true
+ stop when result is known continue when it is not
+ make progression toward termination and keep the picture true with each loop
+ **repetend** -- the body of the loop

##Invariant
+ each piece of a program should be understandable without all of the other parts
+ these parts should then be able to be put together and still have the same meaning

###Loop invariant
+ should be true before and after each iteration of the loop
+ documented like so:

```java
//invariant
while ( condition ) {
```

####Loopy questions
1. Does it start right?
2. Does it stop right?
3. Does repetend make progress?
4. Does repetend keep invariant true

##Ranges
+ b[m..n] means the values from m to n inclusive
    + number of elements = Follower - First
        + for [2..1] = 2 - 2 = 0
        + for [2..4] = 5 - 2 = 3

