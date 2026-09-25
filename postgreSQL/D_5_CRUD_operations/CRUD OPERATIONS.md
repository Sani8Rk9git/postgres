# CRUD OPERATIONS

- CRUD operations in database are the 4 basic operations that can be performed on the data.
    - Create
    - Read
    - Update
    - Delete

### Creating a table

- A table is a collection of related data held in the database
- A table contains rows and columns

```
CREATE TABLE <name> (
<col_1> <datatype> <constraint>,
<col_2> <datatype> <constraint>,
....
);
```
- column names are separated with commas
- datatype tells what type of values the column will contain
    - INT
    - VARCHAR(<value>)
        - variable character
        - it will assign memory blocks according to the length of input.
        - maximum characters entered is <value>

- to see the table in pgadmin
    - click dropdown of database
    - schema
    - public
    - tables

```
SELECT
column_name,
data_type,
character_maximum_length,
is_nullable
FROM information_schema.columns
WHERE table_schema='public'
AND table_name = '<table_name>';
```
- in the command line
    - ```\d <name>;```
    - name is the table name

### Inserting the data in the table

```
INSERT INTO <name>(col1 , col2 , ...)
VALUES (val1 , val2 , ...);
```
- enter the value in the sequence as the columns are written
- use single quotes in the characters
- column names are written without quotes

### To enter multiple values

```
INSERT INTO <name>(col1 , col2 , ...)
VALUES
(val1 , val2 , ...),
(val1 , val2 , ...),
...
;
```
- if we enter values to all the columns in the sequence as defined in the table
```
INSERT INTO <name>
VALUES
(val1 , val2 , ...),
(val1 , val2 , ...),
...
;
```
- we do not need to specify the columns name

### Reading data from the table

- ```SELECT * FROM <name>;```
    - name is the name of the table
    - \* fetches all the columns

- if we want some specific columns
    - ```SELECT col FROM <name>;```
    - ```SELECT col1, col2 ,... FROM <name>;```

### Updating the data in the table

```
UPDATE <table_name>
SET <col_name> = <value>
WHERE <col> = <value>;
```
- the where clause is used to add a condition
    - it tells for which row we need to change the value
- set make the col value to given value

### Delete data from the table

```
DELETE FROM <table>
WHERE <col>=<value>;
```

- to open the file of sql
- query tool
- open file
- You don't need to save the .sql file for the database change to exist.
- The .sql file only saves the text/code of your query so you can use it again later.

