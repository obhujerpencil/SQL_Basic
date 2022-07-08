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
#### Inserting Values
```bash
insert into EmployeeDemographics values
(1001, 'Jim', 'Halpert', 30, 'Male'),
(1002, 'Pam', 'Beasley', 30, 'Female'),
(1003, 'Dwight', 'Schrute', 29, 'Male'),
(1004, 'Angela', 'Martin', 31, 'Female'),
(1005, 'Toby', 'Flenderson', 32, 'Male'),
(1006, 'Michael', 'Scott', 35, 'Male'),
(1007, 'Meredith', 'Palmer', 32, 'Female'),
(1008, 'Stanley', 'Hudson', 38, 'Male'),
(1009, 'Kevin', 'Malone', 31, 'Male')

insert into EmployeeSalary values
(1001, 'Salesman', 45000),
(1002, 'Receptionist', 36000),
(1003, 'Salesman', 63000),
(1004, 'Accountant', 47000),
(1005, 'HR', 50000),
(1006, 'Regional Manager', 65000),
(1007, 'Supplier Relations', 41000),
(1008, 'Salesman', 48000),
(1009, 'Accountant', 42000)
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
![](images/Group%20%26%20Order%20.jpg)

### Bye Byeee.,..
![](images/gif_mysql.gif)
