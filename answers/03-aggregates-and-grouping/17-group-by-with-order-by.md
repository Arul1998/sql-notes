# Lesson 17 Answer: GROUP BY with ORDER BY

## Exercise

Display each department and the number of employees in it. Name the calculated column `EmployeeCount`, and sort from the largest employee count to the smallest.

## Sample Table

### Employees

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | IT | 30000 |
| Sara | Finance | 52000 |
| Adam | Sales | 34000 |

## Answer

```sql
SELECT
    Department,
    COUNT(*) AS EmployeeCount
FROM Employees
GROUP BY Department
ORDER BY EmployeeCount DESC;
```

## Expected Result

| Department | EmployeeCount |
|---|---:|
| IT | 2 |
| Finance | 2 |
| Sales | 1 |

IT and Finance are tied, so SQL Server may return those two rows in either order.
