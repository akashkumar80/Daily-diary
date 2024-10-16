# Day 15:-2 July 2024

## Generics and Lambda Expressions
Lambda expressions in Java 8 are a significant feature that allows for a clear and concise way to represent one method interface using an expression. They are essentially expressions that implement instances of functional interfaces, which are interfaces with a single abstract method.

### Advantages
**1.Less Code:** Lambda expressions reduce the amount of code, making it more readable and maintainable.
**2.Functional Programming:** They facilitate functional programming by enabling functions to be treated as method arguments, or passed around as objects.
**3.Ease of Use:** They can be used easily with the Collection framework, such as in forEach methods to iterate, filter, and extract data.

### Syntax 
```java
(parameter1, parameter2) -> expression
```

### Example
```java
// A functional interface with a single abstract method
interface FuncInterface {
void abstractFun(int x);
}

class Test {
public static void main(String args[]) {
// Lambda expression to implement the abstract method
FuncInterface fobj = (int x) -> System.out.println(2 * x);

// Calling the method with a lambda expression
fobj.abstractFun(5);
}
}
```