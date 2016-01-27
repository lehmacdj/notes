# Trees
+ Each tree may have zero or more successors
+ Each node has exactly one predecessor except the root, which has none
+ All nodes are reachable from root

## Binary tree
+ a treee in which each node can have at most two children
    + left and right

## Terminology
+ Subtrees - trees that start at a node of depth greater than the root
+ depth - length of path from root
+ height - lenghth of path from leaves ( the longest path)
+ leaves - empty child
+ ancestor / descendent - stuff in a tree

## Applications of trees
###Programming languages
+ most languages have a recursive / hierarchical structrure
+ This structure is implicit in ordinary textual representation
+ Recursive structure can be made explicit by representing sentences in the language as trees
+ ASTs are easier to optimize etc
+ parser can convert text to AST

## Recursion
+ Trees are defined recursively, 
+ So recursive methods can be written to process trees in an obvious way
+ Base case - empty tree / leaf
+ Recursion - process all children

## Binary tree search
+ searches for a value in a tree.
+ equivalent to binary search in a list

### Binary search tree
+ enables a faster searching algorithm through use of an ordered tree
+ the tree must be ordered with no duplicate values
+ in every subtree
    + all left descendents must come before the node
    + all right descendents must come after the node
+ search is much faster

#### Building a binary search tree
+ search for an item
+ put the new item where the element should be
+ if nodes are inserted in increasing order a binary search tree it degenerates to a list
+ BST works great as long as data arrives in a random order
+ it is kind of important to keep the tree balanced

#### Printing
1. print left nodes
3. print current node
2. print right nodes

+ since elements are ordered this will yield a tree in alphabetical order

#### Tree traversal
+ in order traversal
    + left, root, right
+ pre order traversal
    + root, left, right
+ post order traversal
    + left, right, root
+ level order
    + everything on one level then on the next level
    + requires a queue
    + not recursive


