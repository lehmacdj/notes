# Threads and Concurrency
## Moore's Law
+ computer speeds and memory densities nearly double each year

### Problems
+ Power dissipation rises as square of clock speed 
+ chips were heading toward melting down
+ multicore chips, with four cpus on one chip even if we run each at half the speed we can do more computations

### Super clusters 
+ sometimes programs want to execute on multiple computers

## Processes
+ The computer provides abstract processes that virtualize the processors into multiple cores

## Threads
+ a virtualization in the virtual machine
+ several threads run all of the time
   + garbage collection
    + GUIs have a searate thread that listens for events and "dispatches" upcalls

### Entry points
+ each thread needs an entry point

## Concurrency
+ A program that has single threads running

### Problems
+ they see the same data and can interfere with each other, if one thread is modifying a complex structure like a head while another is trying to read it
+ race conditions
+ deadlock

## Thread Class
+ Threads are instances of the class thread
+ JVM creates the thread that executes your main method
+ Threads have a priority
+ higher priority threads are executed preferentially
+ by default threads have the same priority as the thread that created them
+ use start method to create a new thread
+ terminating threads can lead to broken internal structures
+ pausing threads is relatively easy

### Race conditions
+ When doing things at the same the same time they race to complete the action
+ can lead to nondeterministic information or lost data
+ often cause bugs
+ common cause for blue screens null pointer exceptions, damaged data structures

### Synchronization
+ a way to eliminnate race conditions
+ a synchronization barrier
+ like a lock
+ only one thread can obtain a lock

### Starvation
+ can lead to low priority threads not getting access to the lock

### Deadlock
+ a downside of locking
+ when two threads are waiting for one-another 
+ both threads want the lock that the other holds
+ always involve graphs that contain cycles
+ locks need to be mutually exclusive
+ no sharing of the objects being locked
+ the application won't give up and go away
+ there are no mechanisms for one thread to take locked resources away from another thread
    + ie preemtion

#### Dealing with deadlocks
+ design code to aquire a lock use it then promptly release it
+ aquire locks in some fixed order
+ don't synchronize huge blocks of code

### Locks
+ Every object has built in locks
+ depite this lots of pelple like making their own explicit locks

### Thread Safety
+ Code is thread safe if only one program can be in the method at a time

### Producer / Consumer
+ producer: wait until not full; add a loaf; this.notifyAll()
+ while empty wait; remove a loaf; this.notifyAll()

