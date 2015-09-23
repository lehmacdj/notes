#Subspaces
+ a subset of R^n
+ A line could be a subspace of R^n
+ a subspace consists of the span of some vectors

##Conditions for a subspace
+ if **u**, **v** in U then **u** + **v** is also in U
+ the same is true for scalar multiplication
+ **0** is in U

##Column space of A
+ the span of the column vectors of A
+ all vectors **b** suchthat A**x** = **b** has a solution

##Null subspace of R^n
+ all x ∈ R^n such A**x** = **0**
+ solutions of the homogenous system

##Basis of a subspace
+ a basis for a subspace is a set that is not redundant and represents the vector subspace
+ v1 ... vk is basis of V if 
    + v = span{v1...vk}
    + v1...vk are linear independent

##Uniqueness
+ most subspaces have many different basises
+ if V is zero subspace V = {**0**}
    + basis of V is the empty set

##The following are equivalent
+ any two basises of a subspace have the smae number of vectors
    + the size of any basis is called the dimenison of V (dimV)
+ if v1...vk ∈ V such that span{v1..vk} = V k ≥ dimV
    + if k = dimV then v1...vk are linearly independent
+ if v1...vk ∈ V and v1..vk are linear independent, k &lt;= dimV
    + if k = dimV they span R^k

##To find a subspace
+ row reduce a matrix that consists of the vectors
+ if any of the vectors are linearly independent one of those vectors can be dropped
+ it doesn't matter what vector is dropped as long as none of the resulting vectors are dropped and none of the vectors that were dropped were linearly independent

##Rank
+ dimV of the subspace spanned by the column vectors of V

##Nul space of A
+ all vectors v such that Av = 0
+ check that this is a subspace
+ if A is a n * m matrix
    + nul A ∈ R^m colA ∈ R^n

###The basis fo rnul A
+ nulA consists of the solution to the homogenous equation

##Rank Theorem
+ for an n * m matrix A
    + dimColA + domNulA = m
