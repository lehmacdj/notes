# Types

## Aside: Lazy evaluation vs Eager evaluation
+ Eager evaluation f(x) -> b(x) of f a
    1. evaluate a to a canonical value a'
    2. substitute a' for x in b(x)
    3. evaluate b(a') to a canonical value
+ Lazy evaluation
    1. substitute b(a)
    2. evaluate b(a) to a canonical expression
+ OCaml uses eager evaluation
+ All data types including lists are evaluated eagerly

## OCaml Type system
+ Basic types
    + int
    + bool
    + char
    + string
    + 'a * 'b
    + 'a -> 'b
    + 'a + 'b
    + list, tree, ...
+ All of these types have the diverging ⟂ element
    + even bool = {true, false, ⟂}
+ variant types ('a + 'b)
    + things of type 'a or 'b with a value of the corresponding type
+ Type variables
    + `fun x -> x`
        + is of type 'a -> 'a
    + `fun x -> (x, x)`
        + is of type 'a -> 'a * 'a
