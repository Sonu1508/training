# JDBC ASSIGNMENT
## Q.1.WHAT IS JDBC?
ANS:JDBC or Java Database Connectivity is a Java API to connect and execute the query with the database. It is a specification from Sun microsystems that provides a standard abstraction(API or Protocol) for java applications to communicate with various databases. It provides the language with java database connectivity standards. It is used to write programs required to access databases. JDBC, along with the database driver, can access databases and spreadsheets. The enterprise data stored in a relational database(RDB) can be accessed with the help of JDBC APIs.

## Q.2.HOW TO CONNECT JAVA APPLICATION TO JDBC?
ANS:There are 5 steps to connect any java application with the database using JDBC. These steps are as follows:
- Register the Driver class
- Create connection
- Create statement
- Execute queries
- Close connection
1) Register the driver class
The forName() method of Class class is used to register the driver class. This method is used to dynamically load the driver class.
Syntax of forName() method
public static void forName(String className)throws ClassNotFoundException  

2) Create the connection object
The getConnection() method of DriverManager class is used to establish connection with the database.
Syntax of getConnection() method
1) public static Connection getConnection(String url)throws SQLException  
2) public static Connection getConnection(String url,String name,String password)  
throws SQLException  
3) Create the Statement object
The createStatement() method of Connection interface is used to create statement. The object of statement is responsible to execute queries with the database.
Syntax of createStatement() method
public Statement createStatement()throws SQLException  
4) Execute the query
The executeQuery() method of Statement interface is used to execute queries to the database. This method returns the object of ResultSet that can be used to get all the records of a table.
Syntax of executeQuery() method
public ResultSet executeQuery(String sql)throws SQLException  

5) Close the connection object
By closing connection object statement and ResultSet will be closed automatically. The close() method of Connection interface is used to close the connection.
Syntax of close() method
public void close()throws SQLException  

## Q.3.DESCRIBE THE ARCHITECTURE OF JDBC?
ANS:![image](https://user-images.githubusercontent.com/95277583/204099993-f6c6aade-857b-4ef3-9e41-ea22ceab7ce8.png)
- Application: It is a java applet or a servlet that communicates with a data source.
- The JDBC API: The JDBC API allows Java programs to execute SQL statements and retrieve results. Some of the important classes and interfaces defined in JDBC API are as follows:
- DriverManager: It plays an important role in the JDBC architecture. It uses some database-specific drivers to effectively connect enterprise applications to databases.
- JDBC drivers: To communicate with a data source through JDBC, you need a JDBC driver that intelligently communicates with the respective data source.

## Q.4.DESCRIBE THE COMPONENTS OF JDBC?
ANS:- Components of JDBC 
There are generally four main components of JDBC through which it can interact with a database. They are as mentioned below: 

1. JDBC API: It provides various methods and interfaces for easy communication with the database. It provides two packages as follows, which contain the java SE and Java EE platforms to exhibit WORA(write once run anywhere) capabilities.

java.sql.*;
2. It also provides a standard to connect a database to a client application.

3. JDBC Driver manager: It loads a database-specific driver in an application to establish a connection with a database. It is used to make a database-specific call to the database to process the user request.

4. JDBC Test suite: It is used to test the operation(such as insertion, deletion, updation) being performed by JDBC Drivers.

5. JDBC-ODBC Bridge Drivers: It connects database drivers to the database. This bridge translates the JDBC method call to the ODBC function call. It makes use of the sun.jdbc.odbc package which includes a native library to access ODBC characteristics.

## Q.5.What is the role of the JDBC DriverManager class?
The DriverManager class acts as an interface between user and drivers. It keeps track of the drivers that are available and handles establishing a connection between a database and the appropriate driver. The DriverManager class maintains a list of Driver classes that have registered themselves by calling the method DriverManager.registerDriver().


