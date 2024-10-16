# Day 8:-21 June 2024

## Polymorphism
The word ‘polymorphism’ means ‘having many forms’. In simple words, we can define Java Polymorphism as the ability of a message to be displayed in more than one form. In this article, we will learn what is polymorphism and its type.
### Types of Polymorphism
In Java Polymorphism is mainly divided into two types: 
<ul>
  <li>Compile Time Polymorphism</li>
  <li>RunTime Polymorphism</li>
</ul>

### Method Overloading
When there are multiple functions with the same name but different parameters then these functions are said to be overloaded.
```java
// Java Program for Method overloading

// Class 1
// Helper class
class Helper {

    // Method with 2 integer parameters
    static int Multiply(int a, int b)
    {
        // Returns product of integer numbers
        return a * b;
    }

    // Method 2
    // With same name but with 2 double parameters
    static double Multiply(double a, double b)
    {
        // Returns product of double numbers
        return a * b;
    }
}

// Class 2
// Main class
class GFG {
    // Main driver method
    public static void main(String[] args)
    {
        // Calling method by passing
        // input as in arguments
        System.out.println(Helper.Multiply(2, 4));
        System.out.println(Helper.Multiply(5.5, 6.3));
    }
}
```