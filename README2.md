## Second assignment for the SQL

**1.** Write a SQL statement to create a simple table countries including columns country_id,country_name and region_id.

`CREATE TABLE countries( country_id varchar(5), country_name varchar(255), region_id decimal(5,0));`

**2.** Write a SQL statement to create a simple table countries including columns country_id,country_name and region_id which already exist.

`CREATE TABLE countries( country_id varchar(5), country_name varchar(255), region_id decimal(5,0)  );`

**3.** Write a SQL statement to create the structure of a table dup_countries similar to countries.

`CREATE TABLE dup_countries AS SELECT * FROM countries WHERE 1=2; `

