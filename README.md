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
