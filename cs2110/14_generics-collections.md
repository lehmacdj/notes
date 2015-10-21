# Generics
+ Before generics objects were used instead.
+ Type casts were nescessary to use methods of the type that was acutally stored in the collection
+ Arrays already had generic like syntax
+ Generics were eventually added 
+ collections can use to eliminate the cast using type paramenters
+ uses type erasure to only require changes to the source code, class files still work the same.
+ `List<String>` is implemented by `ArrayList<String>`
+ `LinkedList<String>` is not a subtype of `LinkedList<Object>` 
+ For Arrays `String[]` is a subtype of `Object[]`

## Wildcards
+ it is possible to use wild cards with `Collection<?>`
+ It means a `Collection` of unknown values
+ values can't be added to collections with a wildcard type parameter

### Bounded wildcards
+ `? extends T`
+ can only be used on things that extend `T`
+ allows general functions that can't be used on absolutely anything
+ within the constraint of the wildcard gives extra info
+ outside of the constraint checks to make sure that constraint is followed

## Generic Method
+ Methods with generic parameters
+ an alternative to wildcards
+ more restrictive but allows adding to the generic collection, etc.
