#Types

##Type Systems (The big picture)

###Dynamically typed code
+ Error prone
+ allows great flexibility

###Statically typed code
+ Annoying to programmers who know other invariants of the code
+ Safer
+ Still has some complicated cases

##Arrays
+ Notation
    + `Object[] v = new Object[3]`
+ Store multiple of some type of object
+ arrays are statically sized
+ when initialized the objects within the array are initialized to `null`
+ only methods declared in the class the array was declared of can be declared
+ however when methods are executed the subclasses override of that method is executed if it exists
    + actual method calls are still determined by the bottom up rule

##Type Checking
+ c.m() is legal only if m is declared in C or one of its superclasses
    + where c is of class C

##Type Casts
+ Casts can occur up or down the type hierarchy
    + Casts only succeed if the object contains a partition for the object it is being cast to
+ doesn't change the object; only changes the view of the object by the object

###Implicit casts
+ only occur up the type hierarchy
+ up casts can never fail so this occurs silently in the program as needed

##instanceof
