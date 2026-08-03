# Lesson 4: AND

`AND` combines conditions. Every condition must be true for a row to appear.

Imagine this `Employees` table:

| EmployeeId | EmployeeName | Department | Age | Salary |
|---:|---|---|---:|---:|
| 1 | Arul | IT | 28 | 36000 |
| 2 | Priya | Finance | 32 | 45000 |
| 3 | John | IT | 25 | 30000 |
| 4 | Sara | Finance | 35 | 52000 |
| 5 | Adam | Sales | 29 | 34000 |

To display IT employees earning at least £35,000:

```sql
SELECT EmployeeName, Salary
FROM Employees
WHERE Department = 'IT'
  AND Salary >= 35000;
```

Both conditions must be true:

- The department must be IT.
- The salary must be at least £35,000.

SQL generally follows this pattern:

```sql
SELECT column_name
FROM table_name
WHERE condition1
  AND condition2;
```

## Exercise

Write a query that displays `EmployeeName`, `Age`, and `Salary` for employees aged at least 30 and earning more than £40,000.
