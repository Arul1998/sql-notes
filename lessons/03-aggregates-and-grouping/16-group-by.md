# Lesson 16: GROUP BY

`GROUP BY` creates one result row for each group.

Imagine this `Employees` table:

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | IT | 30000 |
| Sara | Finance | 52000 |
| Adam | Sales | 34000 |

To count employees in each department:

```sql
SELECT
    Department,
    COUNT(*) AS EmployeeCount
FROM Employees
GROUP BY Department;
```

A selected column must normally be:

- included in `GROUP BY`; or
- used inside an aggregate such as `COUNT`, `SUM`, `AVG`, `MIN`, or `MAX`.

SQL generally follows this pattern:

```sql
SELECT group_column, aggregate_function(column_name)
FROM table_name
GROUP BY group_column;
```

## Exercise

Display each department and its average salary. Name the average column `AverageSalary`.
