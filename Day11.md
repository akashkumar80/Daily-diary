# Day 11:-26 June 2024

# Exception Handling

## Activity:-
Handled exceptions using try-catch blocks and performed basic file operations.

## Exceptions
Exception Handling in Java is one of the effective means to handle runtime errors so that the regular flow of the application can be preserved. Java Exception Handling is a mechanism to handle runtime errors such as ClassNotFoundException, IOException, SQLException, RemoteException, etc.
#### Major reasons why an exception Occurs
<ul>
    <li>Invalid user input</li>
    <li>Device failure</li>
    <li>Loss of network connection</li>
    <li>Physical limitations (out-of-disk memory)</li>
    <li>Code errors</li>
    <li>Out of bound</li>
    <li>Out of bound</li>
    <li>Null reference</li>
    <li>Type mismatch</li>
    <li>Opening an unavailable file</li>
    <li>Database errors</li>
    <li>Arithmetic errors</li>
</ul>

```java
import java.io.*;

class GFG {
    public static void main (String[] args) {
      int a=5;
      int b=0;
        try{
          System.out.println(a/b);
        }
      catch(ArithmeticException e){
        e.printStackTrace();
      }
    }
}
```