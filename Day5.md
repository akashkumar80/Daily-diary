# Day 5:-18 June 2024

## Introduction to OOPs Concept
Object-Oriented Programming is a methodology or paradigm to design a program using classes and objects. It simplifies software development and maintenance by providing some concepts:
<ul>
  <li>Object</li>
  <li>Class</li>
  <li>Inheritance<li>
  <li>Polymorphism</li>
  <li>Abstraction</li>
  <li>Encapsulation</li>
</ul>

![image](images/java-oops.png)

### Object
An Object can be defined as an instance of a class. An object contains an address and takes up some space in memory.
### Class
Collection of objects is called class. It is a logical entity.
A class can also be defined as a blueprint from which you can create an individual object. Class doesn't consume any space.

### Example
```java
//Java Program to illustrate how to define a class and fields  
//Defining a Student class.  
class Student{  
 //defining fields  
 int id;//field or data member or instance variable  
 String name;  
 //creating main method inside the Student class  
 public static void main(String args[]){  
  //Creating an object or instance  
  Student s1=new Student();//creating an object of Student  
  //Printing values of the object  
  System.out.println(s1.id);//accessing member through reference variable  
  System.out.println(s1.name);  
 }  
}  
```
