# Where clause

- Using the WHERE clause, we can get specific data

- we can use relational operators and logical operators also

- we can also use IN , NOT IN 

- we can also use BETWEEN
    - we can provide the range 
    - the ranges are included


- Example

```
SELECT salary FROM employees
WHERE emp_id = 10;
```
```
SELECT * FROM employees
WHERE dept = 'HR';
```

```
SELECT * FROM employees
WHERE salary >= 50000.00;
```

```
SELECT * FROM employees
WHERE dept='IT' OR dept='Sales';
```

```
SELECT * FROM employees
WHERE dept='IT' AND salary >= 50000.00;
```

```
SELECT * FROM employees
WHERE dept IN ('Sales', 'Marketing', 'IT');
```

```
SELECT * FROM employees
WHERE salary BETWEEN 40000.00 AND 50000.00;
```


