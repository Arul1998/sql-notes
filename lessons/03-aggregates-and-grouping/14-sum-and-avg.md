# Lesson 14: SUM and AVG

`SUM` calculates a total, and `AVG` calculates an average.

Imagine this `Employees` table:

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | IT | 30000 |
| Sara | Finance | 52000 |
| Adam | Sales | 34000 |

To calculate the total salary:

```sql
SELECT SUM(Salary) AS TotalSalary
FROM Employees;
```

To calculate the average salary:

```sql
SELECT AVG(Salary) AS AverageSalary
FROM Employees;
```

Both functions can be used in one query:

```sql
SELECT
    SUM(Salary) AS TotalSalary,
    AVG(Salary) AS AverageSalary
FROM Employees;
```

## Exercise

Calculate the total and average salary of employees in the IT department. Name the columns `ITTotalSalary` and `ITAverageSalary`.
