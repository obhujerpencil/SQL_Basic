# SQL_Basic
Create table, Insert values, Select values, Where clause, Group &amp; Order

## Initial Table
```bash
create table EmployeeDemographics(
EmployeeID int,
FirstName varchar(20),
LastName varchar(20),
Age int,
Gender varchar(10)
)

create table EmployeeSalary(
EmployeeID int,
job varchar(20),
Salary int
)
```
![](images/Initial%20Table.jpg)

### Select
```bash
select * from EmployeeDemographics
select top 5 * from EmployeeDemographics
select distinct(Gender) from EmployeeDemographics
select count(EmployeeID) as Number_Of_Employees from EmployeeDemographics
select max(salary) as minWage from EmployeeSalary
select min(salary) as maxWage from EmployeeSalary
select avg(salary) as avgWage from EmployeeSalary
```
![](images/Select%20.jpg)

### Where clause
```bash
select * from EmployeeDemographics where age>30 and gender!='male'
select * from EmployeeDemographics where lastname like '%m%i%'
```
![](images/Where%20clause.jpg)

### Group & Order
```bash
select gender,count(gender) from EmployeeDemographics 
group by gender order by count(gender) desc
```
![](images/)

### Bye Byeee.,..
![](images/gif_mysql.gif)
