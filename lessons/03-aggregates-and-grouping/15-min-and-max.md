# Lesson 15: MIN and MAX

`MIN` returns the lowest value, and `MAX` returns the highest value.

Imagine this `Employees` table:

| EmployeeName | Age | Salary |
|---|---:|---:|
| Arul | 28 | 36000 |
| Priya | 32 | 45000 |
| John | 25 | 30000 |
| Sara | 35 | 52000 |
| Adam | 29 | 34000 |

To find the lowest and highest salaries:

```sql
SELECT
    MIN(Salary) AS LowestSalary,
    MAX(Salary) AS HighestSalary
FROM Employees;
```

You can also use a filter:

```sql
SELECT MAX(Salary) AS HighestITSalary
FROM Employees
WHERE Department = 'IT';
```

## Exercise

Find the youngest and oldest employee ages. Name the result columns `YoungestAge` and `OldestAge`.
