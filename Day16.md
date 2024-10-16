# Day 16:-3 July 2024

## Networking in Java
Java Networking is a concept of connecting two or more computing devices together so that we can share resources.
Java socket programming provides facility to share data between different computing devices.
<b>The java.net package supports two protocols,</b>
1.TCP: Transmission Control Protocol provides reliable communication between the sender and receiver. TCP is used along with the Internet Protocol referred as TCP/IP.
2.UDP: User Datagram Protocol provides a connection-less protocol service by allowing packet of data to be transferred along two or more nodes

### Socket Programming
Java Socket programming is used for communication between the applications running on different JRE.
Java Socket programming can be connection-oriented or connection-less.
Socket and ServerSocket classes are used for connection-oriented socket programming and DatagramSocket and DatagramPacket classes are used for connection-less socket programming.

### Example
##### File:-Myserver.java
```java
import java.io.*;  
import java.net.*;  
public class MyServer {  
public static void main(String[] args){  
try{  
ServerSocket ss=new ServerSocket(6666);  
Socket s=ss.accept();//establishes connection   
DataInputStream dis=new DataInputStream(s.getInputStream());  
String  str=(String)dis.readUTF();  
System.out.println("message= "+str);  
ss.close();  
}catch(Exception e){System.out.println(e);}  
}  
}  
```
##### File:-Myclient.java
```java
import java.io.*;  
import java.net.*;  
public class MyClient {  
public static void main(String[] args) {  
try{      
Socket s=new Socket("localhost",6666);  
DataOutputStream dout=new DataOutputStream(s.getOutputStream());  
dout.writeUTF("Hello Server");  
dout.flush();  
dout.close();  
s.close();  
}catch(Exception e){System.out.println(e);}  
}  
}  
```