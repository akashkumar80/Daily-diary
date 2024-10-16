# Day 7:-20 June 2024

## Inheritance
Inheritance in Java is a mechanism in which one object acquires all the properties and behaviors of a parent object. It is an important part of OOPs (Object Oriented programming system).
### Why use Inheritance
<ul>
  <li>For Method Overriding (so runtime polymorphism can be achieved).</li>
  <li>For Code Reusability.</li>
</ul>

![image](images/inheritance.jpg)

### Syntax
```java
class Subclass-name extends Superclass-name  
{  
   //methods and fields  
}  
```
### Example
```java
class Employee{  
 float salary=40000;  
}  
class Programmer extends Employee{  
 int bonus=10000;  
 public static void main(String args[]){  
   Programmer p=new Programmer();  
   System.out.println("Programmer salary is:"+p.salary);  
   System.out.println("Bonus of Programmer is:"+p.bonus);  
}  
} 
```