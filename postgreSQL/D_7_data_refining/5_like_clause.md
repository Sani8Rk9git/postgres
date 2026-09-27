# Like clause

- It can be used to search for a specified pattern within a column's text data.

```
SELECT * FROM employees WHERE fname LIKE 'A%';
```

- the pattern is case-sensitive

```
SELECT * FROM employees WHERE dept LIKE '__';
```

| Wildcard | Meaning|
| ---------|--------|
| %        | represent 0,1 or multiple characters
| _        | represent exactly single character

