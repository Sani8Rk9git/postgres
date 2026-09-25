# DATATYPES AND CONSTRAINTS

- datatype specify the type of the values that a column can have
- widely used datatypes are:
    - Numeric: INT , DOUBLE , FLOAT , DECIMAL, SMALLINT , BIGINT
        - ```DECIMAL(<max_total_digits> , <max_digits_after_deciaml>)```
    - String: VARCHAR(<value>)
    - Date: DATE
    - CURRENT_DATE(if no date is provided, current date is taken)
    - Boolean: BOOLEAN


## Constraints

- it is a rule applied to a column
- for a single column we can apply multiple constraints

### Types of constraints

1. PRIMARY KEY
    - it uniquely identifies each record in a table
    - must contain unique values
    - cannot contain NULL values
    - a table can have only one primary key column

2. NOT NULL
    - column will not have NULL values

3. DEFAULT 'value'
    - each record has a default value

4. AUTO_INCREMENT
    - automatically increment the values and assign the value
    - use this SERIAL datatype for autoincrement
    - bigserial 

6. UNIQUE
    - allow unique values only

