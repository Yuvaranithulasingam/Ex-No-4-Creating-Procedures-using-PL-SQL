# Ex-4-Creating-Procedures-using-PL-SQL

## Date:

## AIM: 
To create a procedure using PL/SQL.

## STEPS:

1)Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);

2)Create a procedure named as insert_employee data.

3)Inside the procdure block, write the query for inserting the values into the employee table.

4)End the procedure.

5)Call the insert_employee data procedure to insert the values into the employee table.

6)Display the employee table

## PROGRAM:

### Create Table:
```
 create table employeetable(Emp_id number ,Emp_name char (100) , Dept char(20) , Salary number);
```
### Create Procedure:
```
create or replace procedure insert_emp_data as
begin
insert into employeetable(Emp_id,Emp_name,Dept,Salary)
values('1','Yuva','Finance','60000');
insert into employeetable(Emp_id,Emp_name,Dept,Salary)
values('2','Panimalar','IT','55000');
insert into employeetable(Emp_id,Emp_name,Dept,Salary)
values('3','Mena Rossini','HR','50000');
insert into employeetable(Emp_id,Emp_name,Dept,Salary)
values('4','Saranya','IT','55000');
insert into employeetable(Emp_id,Emp_name,Dept,Salary)
values('5','Thanika','Finance','60000');
commit;
end;
/
```
### Call Procedure:
```
 begin
 insert_emp_data;
 end;
 /
```
### Display Table:
```
select * from employeetable;
```

## OUTPUT:

### Create Table:
![image](https://github.com/dineshgl/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121418522/63fcc79e-1452-4985-a7ac-7e43646c5b52)
### Create Procedure:
![image](https://github.com/dineshgl/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121418522/97311185-42b4-4ec6-a977-8144351a923c)
### Call Procedure:
![image](https://github.com/dineshgl/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121418522/cb26eabb-1e6e-4f7b-89bf-0f901a9a0743)
### Display Table:
![image](https://github.com/dineshgl/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121418522/fb633043-b26a-4a17-aab3-74f799385a79)

## RESULT:
Thus, a procedure is created successfully by using PL/SQL.
