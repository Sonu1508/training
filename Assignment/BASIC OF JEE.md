# Basic of JEE Assignment
## Q.1. Explain JEE?
ANS:The Java EE stands for Java Enterprise Edition, which was earlier known as J2EE and is currently known as Jakarta EE. It is a set of specifications wrapping around Java SE (Standard Edition). The Java EE provides a platform for developers with enterprise features such as distributed computing and web services. Java EE applications are usually run on reference run times such as microservers or application servers. Examples of some contexts where Java EE is used are e-commerce, accounting, banking information systems.

- Specifications of Java EE
Java EE has several specifications which are useful in making web pages, reading and writing from database in a transactional way, managing distributed queues. The Java EE contains several APIs which have the functionalities of base Java SE APIs such as Enterprise JavaBeans, connectors, Servlets, Java Server Pages and several web service technologies.

## Q.2.What are the components of J2EE applications?

ANS: The components of J2EE applications include:
1. Client-tier components: Run-on the client machine.
2.  tier components: Run-on the J2EE server.
3. Business tier components: Run-on the J2EE server.
4. Enterprise Information System software (EIS software): Runs on the EIS server.

## Q.3.Describe ORM?
ANS: Object-Relational mapping (ORM) can be described as follows:
The mapped objects in a Java class to the tables of the relational database using metadata describes the database and object mapping. The working method is to transform data from one representation to another.
Advantages are:
- Productivity: Reduced time for data access coding with the help of automatic code creation base on the defined data model.
- Maintainability: All code generated from ORM are well tested. Only the developer is required to create the correct functionality
- Performance: The code generated from ORM completely manages the data access needs of the application. No need to create any data access code. Also, the code is optimized to speed up the data access process.
- Vendor independence: The code generated from ORM does not depend on the vendor. This is to increase the portability of the application.

## Q.4.Define Hibernate?

Ans: Hibernate is an open-source object-relational mapping and query service which facilitates writing Hibernate Query Language (HQL) scripts instead of Structured Query Language (SQL) scripts.

It is a fast and easy process than writing native SQL. Hibernate has more powerful object-oriented contents like associations, inheritance, and polymorphism. Also, it has powerful compositions and collections. Hibernate allows making queries using a Java-based approach.

## Q.5.  How spring is related to J2EE?
ANS:Spring is an open-source application that reduces the complexity of enterprise application development. Spring is based on an inversion of control or dependency injection design patterns.

## Q.6. What are the advantages of using spring for application development?
ANS:
- Plain Old Java Object (POJO) based development facilitates to re-use existing components.
- Possible to reduce development cost by improving the productivity of the application development.
- Improve the testability of application with dependency injection.
- Improve maintainability with reduced code coupling.
- No need to have an application server and works on enterprise service.

## Q.7.Describe the Secure Socket Layer (SSL)?

Answer: The technology that is used to communicate between the web server and the web browser is called Secure Socket Layer (SSL). More specifically, SSL is a protocol that describes how algorithms are to be used in encryption.

The technology establishes an encrypted link between two parties and this link is allowed to secure transmission of sensitive information such as login credentials, credit/debit card information and social security numbers.

## Q.8.What are the design principles for EJB?

Answer: Design principle includes:

- The behavior of the EJB application is specified by interfaces.
- EJB applications are loosely coupled and tired.
- Implementation is hidden from the client-side.
- The EJB container supports the application developer.
- The API to the application is in session tier.
- The API to the data sources is in the entity tier.




