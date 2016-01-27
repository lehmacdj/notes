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
+ not a sorting algorithm
+ pushes the first element to a position where it is greater than anything at a smaller index and smaller than anything at a larger index
+ sorts a single element in a list

### Quicksort 
```java
/** Sorts b[h..k] */
public void QS(int[] b, int h, int k) {
    if (b.length < 2) return;
    
    int j = partition(b, h, k);

    QS(b, h, j - 1);
    QS(b, j + 1, k);
}
```
+ works by partitioning over and over
+ Best case: O(n log(n))
+ worst case: O(n^2)
+ Average case: O(n log(n))
+ the best sorting algorithm

##Mergesort
```java
/** sort b[h..k] */
public void mergesort(int[] b, int h, int k) {
    if (size b[h..k] < 2) return;
    int t = (h + k)/2;
    mergesort(b, h, t);
    mergesort(b, t+1, k);
    merge(b, h, t, k);
}
```
+ Fairly efficient
+ uses linear space since merge creates a copy of half of the array
+ O(n log(n))
+ more space

