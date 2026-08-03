# Lesson 11: NULL Values

`NULL` means a value is missing or unknown.

Imagine this `Employees` table:

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | NULL | 30000 |
| Sara | Finance | 52000 |

To find employees without a department:

```sql
SELECT EmployeeName
FROM Employees
WHERE Department IS NULL;
```

To find employees who have a department:

```sql
SELECT EmployeeName
FROM Employees
WHERE Department IS NOT NULL;
```

Use `IS NULL` or `IS NOT NULL`. Do not use `= NULL`.

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name
WHERE column_name IS NULL;
```

## Exercise

Display `EmployeeName`, `Department`, and `Salary` for employees whose department is not missing. Sort them from the lowest salary to the highest.
