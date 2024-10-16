# Day 14:-1 July 2024

## Collection Framework

Any group of individual objects that are represented as a single unit is known as a Java Collection of Objects. In Java, a separate framework named the “Collection Framework” has been defined in JDK 1.2 which holds all the Java Collection Classes and Interface in it. 

### ArrayList
ArrayList provides us with dynamic arrays in Java. Though, it may be slower than standard arrays but can be helpful in programs where lots of manipulation in the array is needed.
```java
import java.io.*;
import java.util.*;
class GFG {
    public static void main(String[] args)
    {
        ArrayList<Integer> al = new ArrayList<Integer>();
        for (int i = 1; i <= 5; i++)
            al.add(i);
        System.out.println(al);
        al.remove(3);
        System.out.println(al);
        for (int i = 0; i < al.size(); i++)
            System.out.print(al.get(i) + " ");
    }
}
```
### Linked List
The LinkedList class is an implementation of the LinkedList data structure which is a linear data structure where the elements are not stored in contiguous locations and every element is a separate object with a data part and address part.
```java
import java.io.*;
import java.util.*;
class GFG {
    public static void main(String[] args)
    {
        LinkedList<Integer> ll = new LinkedList<Integer>();
        for (int i = 1; i <= 5; i++)
            ll.add(i);
        System.out.println(ll);
        ll.remove(3);
        System.out.println(ll);
        for (int i = 0; i < ll.size(); i++)
            System.out.print(ll.get(i) + " ");
    }
}
```
### Stack
Stack class models and implements the Stack data structure. The class is based on the basic principle of last-in-first-out.
```java
import java.util.*;
public class GFG {
    public static void main(String args[])
    {
        Stack<String> stack = new Stack<String>();
        stack.push("Geeks");
        stack.push("For");
        stack.push("Geeks");
        stack.push("Geeks");
        Iterator<String> itr = stack.iterator();
        while (itr.hasNext()) {
            System.out.print(itr.next() + " ");
        }
        System.out.println();
        stack.pop();
        itr = stack.iterator();
        while (itr.hasNext()) {
            System.out.print(itr.next() + " ");
        }
    }
}
```