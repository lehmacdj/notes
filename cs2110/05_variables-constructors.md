#Variables and Constructors

##Local Variables
+ Local variables can be declared pretty much anywhere
+ Extra storage is allocated
+ local variables are confined to the scope they are declared in
    + scope is defined by curly braces
+ local variables should be defined as close to their first use as possible
+ add statement / assertion comments `// { b <= c }` or `// a description`

##+ bottom up rule / overriding rule
+ the last version of a method declared is the one that is called

##inside-out rule
+ something defined in a construct can be accessed from that scope or a greater scope
+ parameters also participate in this rule
+ works for many different kinds of variables

##this
+ resolves to the current object

##super
+ resolves to the superclass of this object

##Constructors
+ in constructor first initialize superclass fields then initialize classes own fields
+ the first line of a constructor needs to be a constructor
    + if it isn't super(); is called as the first constructor call
