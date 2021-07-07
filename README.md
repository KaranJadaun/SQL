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
