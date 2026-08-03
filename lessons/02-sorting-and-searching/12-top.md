# Lesson 12: TOP

In SQL Server, `TOP` limits the number of rows returned.

Imagine this `Employees` table:

| EmployeeName | Age | Salary |
|---|---:|---:|
| Arul | 28 | 36000 |
| Priya | 32 | 45000 |
| John | 25 | 30000 |
| Sara | 35 | 52000 |
| Adam | 29 | 34000 |

To display the two highest-paid employees:

```sql
SELECT TOP (2) EmployeeName, Salary
FROM Employees
ORDER BY Salary DESC;
```

`ORDER BY` decides which rows are returned. Without it, SQL Server can return any two rows.

SQL generally follows this pattern:

```sql
SELECT TOP (number) column_name
FROM table_name
ORDER BY column_name;
```

## Exercise

Display the three youngest employees. Include `EmployeeName` and `Age`, and use SQL Server syntax.
