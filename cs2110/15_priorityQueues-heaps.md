# Priority Queues and Heaps
##Stacks and Queues
+ restricted lists
+ Stack - LIFO
+ Queue - FIFO
+ These operations are O(1)

## Bag
+ a multiset
+ can store multiple copies of objects

## Priority Queue
+ Bag in which data items are Comparable
+ smaller elements have higher priority
+ remove() returns the element with the highest priority
+ breaks ties arbitrarily

###Purpose
+ Scheduling jobs on a computer
    + default priority = arrive time
    + priority can be changed by operator
+ Scheduling events for an event handler
    + prority = time of occurrence
+ Airline check-in
    + first class, business class, coach
    + FIFO within each class
+ Tasks you have to carry out
    + you determine priority

### Possible implementations
+ queue for each priority level
    + FIFO within each level
    + like airline check-in example
+ unordered list
    + add() - O(1)
    + poll() - O(n)
    + peek() - O(n)
+ ordered list
    + add() - O(n)
    + poll() - O(1)
    + peek() - O(1)

## Heaps
+ concrete data structure
+ very effective for implementing priority queues
+ gives better complexity than ordered or unordered implementation
    + add() - O(log n)
    + poll() - O(log n)
    + peek() - O(1)
    + O(n log n) to process n elements
+ Binary tree with data at each node
+ Heap Order Invariant
    + The least (hightest priority) element of any subtree is at the root of that subtree
+ binary tree is complete
    + every level of the tree is completely filled
    + nodes on bottom level are as far left as possible
+ a heap can be represented by an array
    + number the tree from root down and then from left to right
    + the children of a node k are 2k + 1 and 2k + 2
    + child of k is (k - 1)/2
    + Tree structure is implicit, no need for explicit links

### Heap operations
####add()
1. add e to the end of the array
2. if it invalidates the heap invariant swap with parent
3. repeat until invariant is true

####poll()
1. remove the the root element and return it
2. fill the root with the last element fo the array
3. swap down to the smaller child until it is at the lowest level of the tree

### Changing heap behavior
+ Separate priority from value
    + easy
+ be able to modify the priority
    + hard
+ Heap sort O(log n) sorting algorithm
