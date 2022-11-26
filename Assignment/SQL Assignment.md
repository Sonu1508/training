# SQL Assignment

## Q.1.  Write an SQL query to find the current date-time.
Ans: </br>
SELECT SYSDATE FROM DUAL;

## Q.2. Write an SQL query to join 3 tables.
Ans: </br>
SELECT column1, column2
FROM TableA
JOIN TableB ON TableA.Column3 = TableB.Column3
JOIN TableC ON TableA.Column4 = TableC.Column4;

## Q.3.Write an SQL query to find the employee id whose salary lies in the range of 1000 and 15000.
Ans. </br>
SELECT EmpId, Salary
FROM Emp
WHERE Salary BETWEEN 1000 AND 15000;

## Q 4. Create a customer table.
Ans: </br>
CREATE TABLE customers  
( customer_id number(10) NOT NULL,  
  customer_name varchar2(50) NOT NULL,  
  city varchar2(50)  
);  

## Q.5. Display the name of the current user.
Ans: </br>
show user

## Q.6.Display the names of employees whose name starts with alphabet S.
Ans: </br>
select ename from emp where ename like 'S%';

## Q.7. Display the Employee names for employees whose name ends with alphabet S.
Ans: </br>
select ename from emp where ename like '%S';

## Q.8. Display the names of salesman who earns a salary more than the highest salary of clerk.
Ans: </br>
select ename,sal from emp where job='SALESMAN' and sal>(select
max(sal) from emp
where job='CLERK');

## Q.9.  Display the names of the employees who earn highest salary in their
respective departments.
Ans: </br>
select ename,sal,deptno from emp where sal in(select max(sal) from
emp group by deptno);

## Q.10.Display those managers name whose salary is more than average salary of
his employee?
Ans: </br>
SELECT DISTINCT EMP.ENAME FROM EMP,EMP E WHERE E.SAL <(SELECT AVG(EMP.SAL) FROM EMP
WHERE EMP.EMPNO=E.MGR GROUP BY EMP.ENAME) AND EMP.EMPNO=E.MGR;

## Q.11. what is sql?
Ans:


