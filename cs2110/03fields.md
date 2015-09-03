#Fields, Getters, Setters, Constructors, Testing

##Time Class
```java
/** An instance maintains a time of day */
public class Time {

    private int hr; //time in hours; in 0..23
    private int min; //time in minutes; in 0..59

    /** return the hour of the day */    
    public int getHour() {
        return hr;
    }
    /** return the minute of the hour */
    public int getMin() {
        return min;
    }

    /** = a description of this object */
    public String toString() {

        return hr + ":" + min;
    }

    /** = p, as a string with at least 2 chars
     * --prepend 0 if necessary */
    private String make2(int p) {
        if (0 <= p && p < 10) {
            return "0" + p;
        } else {
            return String.valueOf(p);    
        }
    }
    /** change the hour of the day to h */
    public void setHour(int h) {
        hr = h;
    }

    /** change the minute of the day to m */
    public void setMinute(int m) {
        min = m;
    }
    
    ...
    
}
```
+ invariant -- a description of what the field contains.  Must be enforced by all methods
+ /** **javadoc** -- to be used to describe stuff
+ constructor -- allows custom initialization of a new object

##Constructor
initialize field of a new object so its class invariant is true

###New expression new \<constructor-call>
1. create a new object of class, with default values in fields
2. Execute the constructor-call
3. Give as value of the expression the name of the new Object
###Testing
+ check that every field has the correct value
