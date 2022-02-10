# SQL Query Exercise

Create a database - **“Digital Career Institute”**  
rename it to **dci**  
Hint: Use ALTER DATABASE command with RENAME TO.  
Create  four schemas  - “students”, “courses”, “partners”,  “sales”  
Create at least two tables in each schema, and fill each with at least four rows.  
use all DDL commands in some way from your choice  
-CREATE  
-ALTER  
-DROP  
-TRUNCATE  
-RENAME

## Create Database

`createdb digitalcareerinstitute`
## Rename the database
`alter database digitalcareerinstitute rename to dci;`

`psql dci`

## create four schemas

`create schema students;`

`create schema courses;`

`create schema partners;`

`create schema sales;`

## Creating and inserting rows to tables in students schema
`create table students.studentinfos(first_name varchar(255), family_name varchar(255));`

`insert into students.studentinfos values ('Parisa','Mazinanian'),('Ruli','Afshar'),('Safwan','Kher'),('Sara','Hal');`

`create table students.studentid(id int, dateofregister date);`

`insert into students.studentid values (1,'10-02-2022'),(2,'10-02-2022'),(3,'10-02-2022'),(4,'10-02-2022');`

## Creating and inserting rows to tables in courses schema

`create table courses.courseinfos(name varchar(255), unit int);`

`insert into courses.courseinfos values ('Math',4),('RemoteSensing','6'),('ComputerScience','6');`

`create table courses.courseid(id int, dateofcourse date);`

`insert into courses.courseid values (1,'10-02-2022'),(2,'10-02-2022'),(3,'10-02-2022'),(4,'10-02-2022');`

## Creating and inserting rows to tables in partners schema

`create table partners.partnerinfos(name varchar(255), dateOfPartnership date);`

`insert into partners.partnerinfos values ('Delivery Hero','10-02-2022),('Google','10-02-2022'),('Parisa','10-02-2022'),('Y','10-02-2022');`


`create table partners.suggestedPartnership(name varchar(255), dateOfSuggestion date);`

`insert into partners.suggestedPartnership values ('ZZ','10-02-2022'),('BB','10-02-2022'),('DD','10-02-2022'),('FF','10-02-2022');`

## Creating and inserting rows to tables in sales schema

`create table sales.amountofsale(amount real, dateOfSale date);`

`insert into sales.amountofsale values (1000.30,'10-02-2022),(5000,'10-02-2022'),(6000,'10-02-2022'),(550.20,'10-02-2022');`


## Dropping the table amountofsale created in the sales schema

`drop table sales.amountofsale;`

## change the column name in the suggestedPartnership table

`alter table partners.suggestedPartnership rename column name to companyname;`

## using truncate to remove the values of the partnerinfos table


` truncate table partners.partnerinfos;`