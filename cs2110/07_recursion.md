#Recursion
+ very important to write documentation
+ important to make sure that reccursive method will terminate

##Stack
+ last in first out -- LIFO
+ a stack of things

###Operations
+ push an element onto the its top
+ pop (remove) top element

##Queue
+ first in first out -- FIFO

##Operations
+ append an element
+ remove first element

##Java Runtime
+ uses stacks
+ the stack contains frames
+ a frame goes into the stack
    + contains local variables
    + parameters
    + return info

##Uses of recursion
+ Math use recursion a lot
    + factorials, exponentiation, etc.

##How do we view recursive functions
1. Have a precise spec
2. assume that it does the right thing
3. Look at all other cases and make sure that they get converted to smaller problems of the same kind
3. make sure that method actually returns
