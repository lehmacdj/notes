# Fibonacci numbers
+ Numbers that have useful applications in a number of fields:

## Implementation
+ A simple implementation can be done recursively

```java
/** Returns the nth fibonacci number */
int fib(int n) {
    if (n <= 1) return 1;
    return fib(n-1) + fib(n-2);
}
```

+ This is quite inefficient because f(n) is calculated multiple times
+ in fact it is O(2^n) time

## The golden ratio

