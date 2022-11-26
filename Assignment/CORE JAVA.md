# CORE JAVA ASSIGNMENT
## Q.1.WHAT IS CORE JAVA?
ANS: Java is a programming language and a platform. Java is a high level, robust, object-oriented and secure programming language.
Java was developed by Sun Microsystems (which is now the subsidiary of Oracle) in the year 1995. James Gosling is known as the father of Java. Before Java, its name was Oak. Since Oak was already a registered company, so James Gosling and his team changed the name from Oak to Java.
- A simple program in java
Simple.java
class Simple{  
    public static void main(String args[]){  
     System.out.println("Hello Java");  
    }  
} 


## Q.2.DESCRIBE THE TYPES OF JAVA?
ANS:There are 4 platforms or editions of Java:

1) Java SE (Java Standard Edition)
It is a Java programming platform. It includes Java programming APIs such as java.lang, java.io, java.net, java.util, java.sql, java.math etc. It includes core topics like OOPs, String
, Regex, Exception, Inner classes, Multithreading, I/O Stream, Networking, AWT, Swing, Reflection, Collection, etc.

2) Java EE (Java Enterprise Edition)
It is an enterprise platform that is mainly used to develop web and enterprise applications. It is built on top of the Java SE platform. It includes topics like Servlet, JSP, Web Services, EJB, JPA
, etc.

3) Java ME (Java Micro Edition)
It is a micro platform that is dedicated to mobile applications.

4) JavaFX
It is used to develop rich internet applications. It uses a lightweight user interface API.


## Q.3.DESCRIBE THE FEATURES OF JAVA?
ANS:- Simple: Java is very easy to learn, and its syntax is simple, clean and easy to understand. According to Sun Microsystem, Java language is a simple programming language.
- Object-Oriented: Java is an object-oriented programming language. Everything in Java is an object. Object-oriented means we organize our software as a combination of different types of objects that incorporate both data and behavior.
- Portable: It is a portable language.
- Platform independent: Java is platform independent because it is different from other languages like C, C++, etc. which are compiled into platform specific machines while Java is a write once, run anywhere language. A platform is the hardware or software environment in which a program runs.
- Secured: Java is best known for its security. With Java, we can develop virus-free systems. Java is secured because:
1. No explicit pointer
2. Java Programs run inside a virtual machine sandbox
- Robust: 1.It uses strong memory management.
2. There is a lack of pointers that avoids security problems.
3. Java provides automatic garbage collection which runs on the Java Virtual Machine to get rid of objects which are not being used by a Java application anymore.
4. There are exception handling and the type checking mechanism in Java. All these points make Java robust.
- High Performance: Java is faster than other traditional interpreted programming languages because Java bytecode is "close" to native code. It is still a little bit slower than a compiled language (e.g., C++). Java is an interpreted language that is why it is slower than compiled languages, e.g., C, C++, etc
- Multithreaded: A thread is like a separate program, executing concurrently. We can write Java programs that deal with many tasks at once by defining multiple threads. The main advantage of multi-threading is that it doesn't occupy memory for each thread. It shares a common memory area. Threads are important for multi-media, Web applications, etc.
- Distributed: Java is distributed because it facilitates users to create distributed applications in Java. RMI and EJB are used for creating distributed applications. This feature of Java makes us able to access files by calling the methods from any machine on the internet.


## Q.4. Write a Java program to calculate Permutation and Combination of 2 numbers.</br>
ANS:package EXAMPLE; </br>
import java.util.Scanner; </br>
public class nprandncr { </br>
public static int fact(int nUM) </br>
{ </br>
int fact=1, i; </br>
for(i=1; i<=nUM; i++) </br>
{ </br>
fact = fact*i; </br>
} </br>
return fact; </br>
} </br>
public static void main(String args[]) </br>
{ </br>
int n, r; </br>
Scanner scan = new Scanner(System.in); </br>
System.out.print("Enter Value of n : "); </br>
n = scan.nextInt(); </br>
System.out.print("Enter Value of r : "); </br>
r = scan.nextInt(); </br>
System.out.print("NCR = " +(fact(n)/(fact(n-r)*fact(r)))); </br>
System.out.print("nNPR = " +(fact(n)/(fact(n-r)))); </br>
} </br>
} </br>

## Q.5.DESCRIBE MULTI-THREADING?
ANS: Multithreading is a Java feature that allows concurrent execution of two or more parts of a program for maximum utilization of CPU. Each part of such program is called a thread. So, threads are light-weight processes within a process.
Threads can be created by using two mechanisms : 
- Extending the Thread class 
- Implementing the Runnable Interface
- Thread creation by extending the Thread class
We create a class that extends the java.lang.Thread class. This class overrides the run() method available in the Thread class. A thread begins its life inside run() method. We create an object of our new class and call start() method to start the execution of a thread. Start() invokes the run() method on the Thread object.
PROGRAM:</br>
class MultithreadingDemo extends Thread { </br>
    public void run() </br>
    { </br>
        try { </br>
            System.out.println( </br>
                "Thread " + Thread.currentThread().getId()+ " is running");  </br>
        } </br>
        catch (Exception e) { </br>
            System.out.println("Exception is caught"); </br>
        } </br>
    } </br>
} </br>
 
public class Multithread { </br>
    public static void main(String[] args) </br>
    { </br>
        int n = 5; </br>
        for (int i = 0; i < n; i++) { </br>
            MultithreadingDemo object= new MultithreadingDemo(); </br>
            object.start(); </br>
        } </br>
    } </br>
} </br>
