# Linear dependence
+ vectors are linear depent if they can be added to zero with non-unique weights
+ there exists c1, c2, ..., ck where c1**v1** + c2**v2** + ... + ck**vk** = **0**
+ some homogenous system of equations has unique solution

## One Vector
+ if **v** ≠ **0** => c**v** ≠ **0** => the vector is linear independent
+ if **v** = **0** => linear dependent

## Two Vectors
+ if one vector is **0** => linear dependent
+ if one vecotr is a multiple of the other => linear dependent
+ otherwise => linear independent

## More Vectors
+ if a subset of a set of vectors is linear dependent the full set is linear dependent
+ the order of the vectors does not make a difference

## Genaral Case {v1, v2, ..., vk}
+ The system is linear independent if and only if:
    + **v1** is zero vector
    + There exists some 1 < i ≤ k, where **vi** can be expressed as a linear combination of the previous vectors
+ Proving the reverse:
    + find the last non zero weight
    + move to other side
    + divide by ci
    + now we are expressing that vector as a linear combination of the other vectors
    + this ignores the case of **v1** being the zero vector
+ the system is linear independent if and only if:
    + the RREF of the vector has no pivots in some column
    + the matrix is the matrix that combines all of the vectors
+ if **v1** ... **vk** vectors in ***R***n and k > n
    + {**v1** ... **vk**} is linear dependent
    + because the # of pivots not greater than k

