# Lecture 6 2/18
+ 'a * 'b is and
+ 'a -> 'b is implies
+ A 'a || B 'b is or
+ each of these language structures can represent a logical concept

(... more history of OCaml ...)

## Canonical lists
+ [e1;e2;e3...] is a canonical list
+ [] is the canonical empty list
+ a non empty list is built using the "cons" operator
+ elements can be consed onto the list e1 :: e2 :: []
+ This list is then displayed as [e1;e2]
+ To deconstruct a list the following primitives are included
    + head: hd h::[] ↓ h
    + tail: tl h::t ↓ t

## The entire OCaml type system

### Atomic types
1. unit
2. boolean
3. int
4. char
5. string
6. float
7. exn := "exception"
8. Big_int

### Type constructors
9. product type, e.g. bool * int. The elements are pairs, and repeated pairings
   are tuples, float * float * float
0. -> function space, e.g. bool -> int. Elements can be anonymous functions such
   as fun x -> exp or fun x -> x
1. options (also called variants, p. 103) e.g. L 'a || R 'b
2. lists, e.g. 'a list, elements \[e1;e2;e3;...;en\] (page 11 chapter 3.)
3. records {d1:ty1;d2:ty2;...} like named tuples
4. objects \<id1:ty1;id2:ty2;...\> not studied in lecture
5. polymorphic [> 'id:val1; 'd2:val2; ...] variants won't be used in lecture (in
   a book there is a warning that this type should not be used
6. 'a ty = | case1 of ty | case2 of ty | casen of ty
7. module type T = sig ... end
8. functors module Name (M: ty1n): tyout = structure ... end
9. monitors - chapter 18 - useful for asynchronus computing

## Type theory of OCaml
+ 200+ axioms vs 10 axioms of set theory + 12 axioms of formal logic math
+ *Provides computability*
+ Folk wisdom - "if it type checks it works"
+ Empty type in ocaml: `type void = {void: 'a.'a}`
    + must contain everything, therefore it must not be able to contain anything
