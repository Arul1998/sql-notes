# Lesson 19: WHERE and HAVING

`WHERE` and `HAVING` can be used together.

- `WHERE` filters rows before grouping.
- `HAVING` filters calculated groups after grouping.

Imagine this `Employees` table:

| EmployeeName | Department | Age | Salary |
|---|---|---:|---:|
| Arul | IT | 28 | 36000 |
| Priya | Finance | 32 | 45000 |
| John | IT | 25 | 30000 |
| Sara | Finance | 35 | 52000 |
| Adam | Sales | 29 | 34000 |

Consider only employees aged 30 or older, then show departments with at least two such employees:

```sql
SELECT
    Department,
    COUNT(*) AS EmployeeCount
FROM Employees
WHERE Age >= 30
GROUP BY Department
HAVING COUNT(*) >= 2;
```

Remember this order:

```sql
SELECT
FROM
WHERE
GROUP BY
HAVING
ORDER BY
```

## Exercise

Consider only employees earning at least £35,000. Display each department and its average salary, but only show departments whose average salary is greater than £40,000. Sort the results from the highest average salary to the lowest.
