# Lesson 17: GROUP BY with ORDER BY

Grouped results can also be sorted with `ORDER BY`.

Imagine this `Employees` table:

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | IT | 30000 |
| Sara | Finance | 52000 |
| Adam | Sales | 34000 |

To display departments from the highest average salary to the lowest:

```sql
SELECT
    Department,
    AVG(Salary) AS AverageSalary
FROM Employees
GROUP BY Department
ORDER BY AverageSalary DESC;
```

The query first creates the department groups and then sorts the calculated results.

SQL generally follows this pattern:

```sql
SELECT group_column, aggregate_function(column_name) AS ResultName
FROM table_name
GROUP BY group_column
ORDER BY ResultName DESC;
```

## Exercise

Display each department and the number of employees in it. Name the calculated column `EmployeeCount`, and sort from the largest employee count to the smallest.
