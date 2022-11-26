## PL/SQL ASSINGMENT

## Q.1. What is PL/SQl?
Ans:PL/SQL is a block structured language. The programs of PL/SQL are logical blocks that can contain any number of nested sub-blocks. Pl/SQL stands for "Procedural Language extension of SQL" that is used in Oracle. PL/SQL is integrated with Oracle database (since version 7). The functionalities of PL/SQL usually extended after each release of Oracle database. Although PL/SQL is closely integrated with SQL language, yet it adds some programming constraints that are not available in SQL.
- PL/SQL includes procedural language elements like conditions and loops. It allows declaration of constants and variables, procedures and functions, types and variable of those types and triggers. It can support Array and handle exceptions (runtime errors). After the implementation of version 8 of Oracle database have included features associated with object orientation. You can create PL/SQL units like procedures, functions, packages, types and triggers, etc. which are stored in the database for reuse by applications.

- With PL/SQL, you can use SQL statements to manipulate Oracle data and flow of control statements to process the data.

- The PL/SQL is known for its combination of data manipulating power of SQL with data processing power of procedural languages. It inherits the robustness, security, and portability of the Oracle Database.

- PL/SQL is not case sensitive so you are free to use lower case letters or upper case letters except within string and character literals. A line of PL/SQL text contains groups of characters known as lexical units. It can be classified as follows:


## Q.2.  What is the use of WHERE CURRENT OF in cursors?
We use this clause while referencing the current row from an explicit cursor. This clause allows applying updates and deletion of the row currently under consideration without explicitly referencing the row ID.
Syntax:
UPDATE table_name SET field=new_value WHERE CURRENT OF cursor_name

## Q.3.What is the difference between a mutating table and a constraining table?
ANS: A table that is being modified by the usage of the DML statement currently is known as a mutating table. It can also be a table that has triggers defined on it.
- A table used for reading for the purpose of referential integrity constraint is called a constraining table.

## Q.4. What do you understand by PL/SQL table?
ANS: PL/SQL tables are nothing but objects of type tables that are modeled as database tables. They are a way to provide arrays that are nothing but temporary tables in memory for faster processing.
- These tables are useful for moving bulk data thereby simplifying the process.

## Q.5. When does a DECLARE block become mandatory?
ANS:This statement is used by anonymous blocks of PL/SQL such as non-stored and stand-alone procedures. When they are being used, the statement should come first in the stand-alone file.
