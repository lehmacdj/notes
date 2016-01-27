#GUI (Graphical User Interface)
+ Provides friendly interface between user and program
+ allows event driven or reactive programming
+ often is multi-threaded: different threads of execution can be going on simultaneously

##GUI Packages
+ AWT (Abstract/Awful Window Toolkit)
+ Swing - newer one that reacts builds on AWT

## Adding components to windows
### JFrame
+ A window for adding items

##Trees
+ The gui representation of a thing becomes a tree
+ the tree must be traversed to determine how much space is required for each component

##Graphics class
+ Has methods for painting stuff

##Listeners
###Action Listeners
+ Do something when the object they are registered to is pressed

###MouseListener
+ Listens to mouse inputs
+ MouseInputAdapter implements Mouse Listener
+ It can be used more easily 

###Keyboard listener
+ Pretty much the same

###etc.
+ Pretty much the same

###Multiple listeners
+ Each listener can listen for a different event
+ must be lambda, anonymous class, or inner class so that variables within the class can be referenced

