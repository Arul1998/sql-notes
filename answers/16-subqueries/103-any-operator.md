# Lesson 103 Answer: ANY

## Exercise

Display employees whose salary is greater than at least one salary in the Sales department.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | John | IT | 40000 |
| 2 | Sarah | Sales | 50000 |
| 3 | David | IT | 30000 |

## Answer

```sql
SELECT EmployeeId, EmployeeName, Salary
FROM Employees
WHERE Salary > ANY (SELECT Salary
FROM Employees
WHERE Department = 'Sales');
```

## Expected Result

No rows match: no employee earns more than Sarah's Sales salary of 50000.
