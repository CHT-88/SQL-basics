# SQL-basics
This is the begginig of my SQL studies.
I will add definitions and very basic topics here to assist me with new concepts and fix my knowledge for the future.

Since I don't have an IT background, everything in this repo will be for absolute begginers.



<details><summary> Basic Concepts
</summary>
<p>

**SQL(Structured Query Language):** is a domain-specific language used to facilitate retrieving specific information from databases.

**Database:** Is a container (it can be a file or set of files) to store organized data.
  
**RDBMS (Relational Database Management System):** .

**Table:** A structured list of data of a specific type.

**Schema:** Information about database and table layout and properties.

**Datatype:** A type of allowed data. Every table column has an associated datatype that restricts (or allows) specific data in that column.

**Primary key:** A column (or set of columns) whose values uniquely identify every row in a table.

 
</p>
</details>


<!--
# SQL Statements

<details><summary>SELECT</summary>
<p>

### SELECT
The SELECT statement is used to select data from a database.

  To retrieve all information in the table:
  `
SELECT * FROM table_name; `
  
  To retrieve specific information:
  `SELECT column1, column2, ...
FROM table_name;`
  
### SELECT DISTINCT
The SELECT DISTINCT statement is used to return only different values, in other words, it will exclude duplicate values.

  `SELECT DISTINCT column1, column2, ...
FROM table_name;`
  
### WHERE Clause
The WHERE clause is used to filter records. 
Only records that fulfill a specified condition will be extracted.
  
  `SELECT column1, column2, ...
FROM table_name
WHERE condition;`
  
### SQL AND, OR and NOT Operators
The WHERE clause can be combined with AND, OR, and NOT operators.
  
  
- The AND operator displays a record if all the conditions separated by AND are TRUE.
`SELECT column1, column2, ...
FROM table_name
WHERE condition1 AND condition2 AND condition3 ...; `
- The OR operator displays a record if any of the conditions separated by OR is TRUE.
`SELECT column1, column2, ...
FROM table_name
WHERE condition1 OR condition2 OR condition3 ...;`
- The NOT operator displays a record if the condition(s) is NOT TRUE.
`SELECT column1, column2, ...
FROM table_name
WHERE NOT condition; `
  
</p>
</details>

https://www.w3schools.com/sql/sql_and_or.asp
-->
