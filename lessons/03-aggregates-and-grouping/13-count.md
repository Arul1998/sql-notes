# Lesson 13: COUNT

`COUNT` counts rows.

Imagine this `Employees` table:

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | IT | 30000 |
| Sara | Finance | 52000 |
| Adam | Sales | 34000 |

To count all employees:

```sql
SELECT COUNT(*) AS TotalEmployees
FROM Employees;
```

To count employees in IT:

```sql
SELECT COUNT(*) AS ITEmployees
FROM Employees
WHERE Department = 'IT';
```

- `COUNT(*)` counts rows.
- `AS` gives the result column a readable name.

SQL generally follows this pattern:

```sql
SELECT COUNT(*) AS ResultName
FROM table_name
WHERE condition;
```

## Exercise

Count employees whose salary is at least £40,000. Name the result column `HighSalaryEmployees`.
