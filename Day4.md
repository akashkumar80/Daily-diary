# Day 4:-14 June 2024

## Functions and Methods

### Activities:-
Created functions for various tasks and understood method overloading.
#### Functions:-
Functions are blocks of code designed to perform a specific task and can be called upon within a program. They may accept input parameters and return a value. Functions are a broader concept found in both object-oriented and procedural programming languages.

#### Methods:-
Methods, on the other hand, are similar to functions in that they also perform actions and can take parameters and return values. However, methods are inherently tied to an object or an instance of a class. They can only operate on the data contained within the class they belong to, making them a key concept in object-oriented programming (OOP).

#### Example:-
```java
public class Calculator {
// Method to calculate the sum of two integers
    public int add(int num1, int num2) {
        return num1 + num2;
    }   

    // Main Method
    public static void main(String[] args) {
        int a = 5, b = 10, sum;
        Calculator calculator = new Calculator();
        // Calling the add() method and storing the result in sum variable
        sum = calculator.add(a, b);
        System.out.println("The sum of " + a + " and " + b + " is " + sum);
    }
}
```