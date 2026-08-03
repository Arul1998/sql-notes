# Lesson 6: ORDER BY

`ORDER BY` sorts query results.

Imagine this `Employees` table:

| EmployeeName | Age | Salary |
|---|---:|---:|
| Arul | 28 | 36000 |
| Priya | 32 | 45000 |
| John | 25 | 30000 |
| Sara | 35 | 52000 |
| Adam | 29 | 34000 |

To sort salaries from lowest to highest:

```sql
SELECT EmployeeName, Salary
FROM Employees
ORDER BY Salary ASC;
```

- `ASC` means ascending order.
- `DESC` means descending order.
- `ASC` is the default and can be omitted.

To sort salaries from highest to lowest:

```sql
SELECT EmployeeName, Salary
FROM Employees
ORDER BY Salary DESC;
```

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name
ORDER BY column_name ASC;
```

## Exercise

Display `EmployeeName`, `Age`, and `Salary` for employees earning at least £36,000. Sort them from the highest salary to the lowest.
