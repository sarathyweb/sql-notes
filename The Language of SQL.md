
# 1. Relational Databases and SQL

There are three major components of SQL
1. DML
- DML stands for Data Manipulation Language
- This component allows us to insert, delete, retrieve and update data from a database
2. DDL
- DDL stands for Data Definition Language
- This component allows to create and modify database schema
3. DCL
- DCL stwnds for Data Control Language
- It provides ACL for the database
<br />

- SQL is decorative language
- Primary key is used to uniquely identify a row in a SQL table
- Primary keys are usually sequentially generated using auto increment
- Foreign keys are used to link two tables using a primary key of one of those tables
<br />

## SQL Data Types
- Numeric data types include bits, integers, floats, decimals and real numbers
- A Bit can be either 0 or 1
- Bit data type is usually used to set an attribute either true (1) or false (0)
- Integers doesn't have any decimal places
- Floats and decimals can have decimal precision
- Floats stores only the approximate value while decimal stores the exact same value
- Floats uses 32 bits while real uses 64 bits to represent a number
- Character data should be surrounded by single quotes
- char represents characters with fixed length while varchar represents variable length 
- Data/time data types are used to represent date and time
- date/time data should be surrounded by single quotes

## NULL Values
- A primary key cannot be null
- When designing a database schema, we can set whether the column can have null values or not

# 2. Basic Data Retrieval
- The SELECT statement is used to retrieve data from a database
- "*" means all columns

SELECT * FROM Customers -> display all columns from table customers

SELECT FirstName FROM Customers -> display all data from the column FirstName

- We can specify multiple column names in the SELECT statement
- If we want to select more than one column from a table, the column names must be separated by commas
- If the column name contains a space, surround the column name with square brackets for SQL server or ` characters for MySQL and double quotes for Oracle

## Full syntax of SELECT statement
SELECT columnlist 
FROM tablename
WHERE condition
GROUP BY condition
HAVING condition
ORDER BY condition
- The columnlist can include functions
- The FROM clause specifies the data source
- The WHERE clause specifies logic

