# Lesson 18: HAVING

`HAVING` filters grouped results after `GROUP BY`.

Imagine this `Employees` table:

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | IT | 30000 |
| Sara | Finance | 52000 |
| Adam | Sales | 34000 |

To display departments with at least two employees:

```sql
SELECT
    Department,
    COUNT(*) AS EmployeeCount
FROM Employees
GROUP BY Department
HAVING COUNT(*) >= 2;
```

- `WHERE` filters individual rows.
- `HAVING` filters groups created by `GROUP BY`.

SQL generally follows this pattern:

```sql
SELECT group_column, aggregate_function(column_name)
FROM table_name
GROUP BY group_column
HAVING aggregate_function(column_name) condition;
```

## Exercise

Display each department and its average salary, but show only departments whose average salary is greater than £40,000. Name the calculated column `AverageSalary`.
