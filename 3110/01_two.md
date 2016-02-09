# Intro to OCaml

### Other functional languages
+ lisp
+ scheme
+ haskell

+ OCaml has the richest type system of all of these
+ No programming language ever dies, there are tons of obscure languages that
  still exist today

## OCaml computation system
+ A well formed string of ocaml symbols is called an expression
+ an expression that cannot be reduced is a canonical expression or value
+ an expression that can be reduced is a non-canonical expression

### Values
+ Some expressions are called values or canonical expressions
    + no longer reducible by computation rules
+ what are values
    + 0 is a value
    + 1 + 2 is not a value
    + true is a value
    + 0 = 0 is not
    + fun x -> x is a value, fun x -> x * x is also a value
    + (fun x -> x + 1) 0 is not a value because it can be evaluated to 0 + 1 = 1

#### Types of values
+ Single value
+ N-Tuple
+ Record (Dictionary)
+ Functions

##### Functions
+ a function is a value
+ functions are irreducible
+ when a function is applied to a value it is reducible

### Reducing expressions to values
+ Rule-fst fst(a, b) ↓ a
+ Rule-snd snd(a, b) ↓ b
+ fun x -> x * x * 0 is a reduced function
+ fun x -> ⟂ 1 ↑ means that a function does not complete

