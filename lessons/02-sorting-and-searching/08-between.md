# Lesson 8: BETWEEN

`BETWEEN` checks whether a value is inside a range. Both boundary values are included.

Imagine this `Employees` table:

| EmployeeName | Age | Salary |
|---|---:|---:|
| Arul | 28 | 36000 |
| Priya | 32 | 45000 |
| John | 25 | 30000 |
| Sara | 35 | 52000 |
| Adam | 29 | 34000 |

To display employees earning from £35,000 through £50,000:

```sql
SELECT EmployeeName, Salary
FROM Employees
WHERE Salary BETWEEN 35000 AND 50000;
```

This is the same as:

```sql
WHERE Salary >= 35000
  AND Salary <= 50000;
```

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name
WHERE column_name BETWEEN lower_value AND upper_value;
```

## Exercise

Display `EmployeeName` and `Age` for employees aged from 28 through 35. Sort the results from oldest to youngest.
