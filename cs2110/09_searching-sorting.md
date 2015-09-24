# Sorting and Searching (A hint at asymptotic complexity)

##Searching
### Binary Search
+ halves the search space on every iteration
+ O(log(n))

### Linear Search
+ Searches through every element consecutively
+ Worst case: O(n)
+ Average case: O(n/2) = O(n)

##Sorting
### Insertion Sort
+ Goes through loop and pushes elements down to a sorted position
+ Best case: O(n)
+ Worst case O(n^2)
+ Expected case O(n^2)

### Selection Sort
+ Set m to the index of minimum of b[i..]
+ swap b[i] and b[m]
+ Best case: O(n^2)
+ Worst case: O(n^2)
+ Expected case: O(n^2)

### Partition algorithm
+ pushes the first element to a position where it is greater than anything at a smaller index and smaller than anything at a larger index
+ 
