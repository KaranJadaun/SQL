# SQL
**SQL is a domain-specific language used in programming and designed for managing data held in a relational database management system, or for stream processing in a relational data stream management system and you can use this language in MySQL database management system.**
#### **SHOW DATABASES** - This is used to show the database.
#### **SHOW TABLES** - This is used to show all the tables of database.
#### **SHOW column_name FROM table_name** - This shows all the columns of the table.
#### **SELECT column_name FROM table_name** - This shows the particular column from the table. You can also do multiple queries with it. You can also select multiple columns from the table by using SELECT column_name, column_name2 FROM table_name.
#### **SELECT * FROM table_name** - This shows all the contents of the tables.
#### **SELECT DISTINCT column_name1, column_name2 FROM table_name** - It basically removes the duplicate entries from the column and shows it. It might make more sense.
#### **SELECT column_name FROM table_name LIMIT (number of records)** - It only shows the top number of records from column_name.
#### **SELECT column_name FROM table_name OFFSET (starting_number) LIMIT (ending_number)** - It only shows the records from starting_number(exluding it) to ending_number from the table_name.
#### **SELECT * FROM table_name ORDER BY column_name** - It is used to sort the given column.
#### **SELECT * FROM table_name WHERE condition_name** - It only shows the column or rows which satisfy the condition given. 
#### ***- Arithmetic Operators are as same as any other programming language.***
#### **SELECT column_name FROM table_name WHERE column_name BETWEEN value1 AND value2** - It only shows the record starting from value1(including it) to value2 from the column_name.
#### **SELECT column_name FROM table_name WHERE condition1 AND condition2** - It is used to combine two or more conditons in where statements and it is true only and only when both conditions are true.
#### **SELECT column_name FROM table_name WHERE condition1 OR condition2** - It is used to combine two or more conditons in where statements and it is true when either one of the statements are true or both are true.
#### **SELECT column_name FROM table_name WHERE condition1 AND (condition2 OR condition3)** - It is used to combine multiple statements in where statements by using both operators AND / OR.
#### **SELECT column_name FROM table_name WHERE condition1 IN (condition2, condition3, condition4)** - It is used to refer something in the conditions, also used instead of multiple or statements.
#### **SELECT column_name FROM table_name WHERE condition1 NOT IN (condition2, condition3, condition4)** - It is used to not refer something in the conditions, also used instead of multiple or statements.
#### **SELECT CONCACT('column_name1', ',', 'column_name2') FROM table_name** -  It is used to concatenate two or more text values and returns the concatenating string.
#### **SELECT CONCACT('column_name1', ',', 'column_name2') AS new_column FROM table_name** - This type of concatination results in a new column.
#### **Upper Function** - This is used to uppercase all the letters of the column_name.
#### **Lower Function** - This is used to lowercase all the letters of the column_name. 
#### **Sqrt Function** - This is used to find square root of the column_name.
#### **Avg Function** - This is used to find the average of the whole column_name.
#### **Power(a,b) Function** - This is used to find the power of a raised to be the power of b.
#### **Sum Function** - This is used to find the sum of the whole column_name.
#### **ASC Keyword** - For ascending order, use with order by.
#### **DESC Keyword** - For descending order, use with order by.
#### **SELECT column_name(s) FROM table_name WHERE column_name LIKE A%** - This is used to show database in a unique manner like this with shows all the entries starting from a in column_name.
#### **Min Function** - This is used to find the minimun number in the column_name.
#### **SELECT table_name.column_name1, table_name.column_name2.... FROM table_name1, table_name2 WHERE table_name1.ID = table_name2.customersID ORDER BY table_name1.ID** - This is a joining feauture that helps into joining two or more table into one temporary table. You can select which column you need from which table. The syntax is written above.\
#### **SELECT tn.column_name1, tn2.column_name2.... FROM table_name1 AS tn, table_name2 AS tn2 WHERE tn.ID = tn2.customersID ORDER BY tn.ID** - You can also customise the name of the table to make it simple for you to write the code. 
#### -The following are the types of JOIN that can be used in MySQL:
####   - INNER JOIN
####   - LEFT JOIN
####   - RIGHT JOIN 
#### **SELECT column_name(s) FROM table1 INNER JOIN table2 ON table1.column_name=table2.column_name** - This inner join feature which returns table when there is a match between them.
#### - Replace INNER JOIN by LEFT OUTER JOIN, RIGHT OUTER JOIN for performing LEFT JOIM and RIGHT JOIN function.
#### To accomplish this, use the UNION and UNION ALL operators.
####   - UNION combines multiple datasets into a single dataset, and removes any existing duplicates.
####   - UNION ALL combines multiple datasets into one dataset, but does not remove duplicate rows.
#### **SELECT column_name(s) FROM table1 UNION SELECT column_name(s) FROM table2** - This Function combines two or more tables and removes the duplicates from the table. It should be of same number of column and have the same type of data.
#### **SELECT column_name(s) FROM table1 UNION ALL SELECT column_name(s) FROM table2** - This Function also combines two or more tables and doesn't remove the duplicates from the table. It also should be of the same number and have the same data data type but if you have one extra column you can use null set.
#### **INSERT INTO table_name VALUES (value1, value2, value3,...)** - You can add a row to a table by using the insert into function amd by adding the values corrosponding to the column(s).
#### **INSERT INTO table_name (column1, column2, column3, ...,columnN) VALUES (value1, value2, value3,...valueN)** - This is an another way of inserting the data into datasets. It is exactly same as INSERT INTO.
#### - If you want to add data to only specific column you can add only on those and the rest of the columns remains null. That will not create an issue.
#### **UPDATE table_name SET column1=value1, column2=value2,... WHERE condition** - This is used to update the table values where conditions maybe id number or any another value which specify the unique row. 
#### **DELETE FROM table_name WHERE condition** - This is used to delete the specific row or column where conditions specify the unique row.
#### - A single database can house hundreds of tables, each playing its own unique role in the database schema.
#### - SQL tables are comprised of table rows and columns. 
#### - Table columns are responsible for storing many different types of data, including numbers, texts, dates, and even files.
#### - CREATE TABLE table_name 
#### (
#### column_name1 data_type(size),
#### column_name2 data_type(size),
#### column_name3 data_type(size),
#### ....
#### column_nameN data_type(size)
#### )
#### - Example - 
#### CREATE TABLE Users
#### (
#### UserID int,
#### FirstName varchar(100), 
#### LastName varchar(100),
#### City varchar(100),
#### PRIMARY KEY(UserId) 
#### ); 
#### - After creating the table you can add values by using INSERT INTO function.
#### - The following are commonly used SQL constraints:
#### NOT NULL - Indicates that a column cannot contain any NULL value.
#### UNIQUE - Does not allow to insert a duplicate value in a column. The UNIQUE constraint maintains the uniqueness of a column in a table. More than one UNIQUE column can be used in a table.
#### PRIMARY KEY - Enforces the table to accept unique data for a specific column and this constraint create a unique index for accessing the table faster.
#### CHECK - Determines whether the value is valid or not from a logical expression.
#### DEFAULT - While inserting data into a table, if no value is supplied to a column, then the column gets the value set as DEFAULT.
#### UserID int NOT NULL AUTO_INCREMENT, PRIMARY KEY (UserID) - This auto increment allows the unique userid to increment its value by 1. It does not require to add unique userid everytime when you insert a row.
#### Example of auto increment - 
#### - CREATE TABLE Users (
#### id int NOT NULL AUTO_INCREMENT,
#### username varchar(40) NOT NULL, 
#### password varchar(10) NOT NULL,
#### PRIMARY KEY(id)
#### );
#### - The ALTER TABLE command is used to add, delete, or modify columns in an existing table.
#### **ALTER TABLE table_name ADD dateofbirth date** - This is used to add a new column in table_name which is named as dateofbirth which have a datatype of data and data inserted in it is NULL.
#### **ALTER TABLE table_name DROP COLUMN dateofbirth** - This is used to delete a column from table_name.
#### **DROP TABLE table_name** - This is used to delete the entire table from the database.
#### **ALTER TABLE table_name RENAME column_name TO column_name1** - This is used to rename the column_name to column_name1.
#### **CREATE VIEW view_name AS SELECT column_name(s) FROM table_name WHERE condition** - This simply creates a view of the table and rest of the codes are same as above.
#### **CREATE OR REPLACE VIEW view_name A SELECT column_name(s) FROM table_name WHERE condition1** - This is used to add column_name if case you forgot it. 
#### **DROP VIEW view_name** - This is used to create the whole view.
