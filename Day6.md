# Day 6:-19 June 2024
## Constructors and this Keyword
### Constructor
In Java, a constructor is a block of codes similar to the method. It is called when an instance of the class is created. At the time of calling constructor, memory for the object is allocated in the memory.
```java
//Java Program to create and call a default constructor  
class Bike1{  
//creating a default constructor  
Bike1(){System.out.println("Bike is created");}  
//main method   
public static void main(String args[]){  
//calling a default constructor  
Bike1 b=new Bike1();  
}  
}  
```
### this keyword
In Java, this is a reference variable that refers to the current object.
Here is given the 6 usage of java this keyword.
<ul>
    <li>this can be used to refer current class instance variable.</li>
    <li>this can be used to invoke current class method (implicitly)</li>
    <li>this() can be used to invoke current class constructor.</li>
    <li>this can be passed as an argument in the method call</li>
    <li>this can be passed as argument in the constructor call.</li>
    <li>this can be used to return the current class instance from the method.</li>
</ul>

```java
class Student{  
int rollno;  
String name;  
float fee;  
Student(int rollno,String name,float fee){  
rollno=rollno;  
name=name;  
fee=fee;  
}  
void display(){System.out.println(rollno+" "+name+" "+fee);}  
}  
class TestThis1{  
public static void main(String args[]){  
Student s1=new Student(111,"ankit",5000f);  
Student s2=new Student(112,"sumit",6000f);  
s1.display();  
s2.display();  
}}  
```