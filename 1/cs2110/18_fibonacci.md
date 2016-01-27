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
+ in fact it is O(phi^n)
+ there are O(n), O(log(n)), and O(1) algorithms
+ O(1): fib(n) = ((phi)^n + ((sqrt(5) - 1)/2)^n)/sqrt(5)

## The golden ratio
+ b / a = a / (b-1); a = 1 then b = the golden ratio
+ golden ratio is about 1.618 or exactly (sqrt(5) + 1)/2
+ represented by phi
