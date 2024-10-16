# Day 10:-25 June 2024

## Abstract Classes and Interfaces

### Abstraction in Java
Abstraction is a process of hiding the implementation details and showing only functionality to the user.
Another way, it shows only essential things to the user and hides the internal details, for example, sending SMS where you type the text and send the message. You don't know the internal processing about the message delivery.
### Ways to achieve Abstraction
<ul>
   <li>Abstract Class</li>
   <li>Interface</li>
</ul>

### Abstract Class
A class which is declared as abstract is known as an abstract class. It can have abstract and non-abstract methods. It needs to be extended and its method implemented. It cannot be instantiated.
```java
abstract class Bike{  
  abstract void run();  
}  
class Honda4 extends Bike{  
void run(){System.out.println("running safely");}  
public static void main(String args[]){  
 Bike obj = new Honda4();  
 obj.run();  
}  
}  
```
### Interface
An interface in Java is a blueprint of a class. It has static constants and abstract methods
The interface in Java is a mechanism to achieve abstraction. There can be only abstract methods in the Java interface, not method body. It is used to achieve abstraction and multiple inheritance in Java.
```java
interface printable{  
void print();  
}  
class A6 implements printable{  
public void print(){System.out.println("Hello");}  
  
public static void main(String args[]){  
A6 obj = new A6();  
obj.print();  
 }  
}  
```