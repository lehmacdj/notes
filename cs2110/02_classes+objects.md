#Classes and Objects
##Methods
+ *function* - returns a value
+ *procedure* - does something

evaluation of a new expression creates an objects

every expression yields a value

variables store addresses to an object

##Class definition

```java
/** description of object */
public class C extends javax.swing.JFrame {
    
    //sample declaration of methods
    
    /** returns the area of the object */
    public int area() {
        return getWidth() * getHeight();
    }
    
    /** make width and height equal */
    public void square() {
        setSize(getHeight(), getHeight());
    }
    
    /** set title to the date */
    public void setDate() {
        setTitle(new java.util.Date().toString());
    }
```

