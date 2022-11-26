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
