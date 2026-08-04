# Lesson 6 Answer: ORDER BY

## Exercise

Display `EmployeeName`, `Age`, and `Salary` for employees earning at least £36,000. Sort them from the highest salary to the lowest.

## Sample Table

### Employees

| EmployeeName | Age | Salary |
|---|---:|---:|
| Arul | 28 | 36000 |
| Priya | 32 | 45000 |
| John | 25 | 30000 |
| Sara | 35 | 52000 |
| Adam | 29 | 34000 |

## Answer

```sql
SELECT EmployeeName, Age, Salary
FROM Employees
WHERE Salary >= 36000
ORDER BY Salary DESC;
```

## Expected Result

| EmployeeName | Age | Salary |
|---|---:|---:|
| Sara | 35 | 52000 |
| Priya | 32 | 45000 |
| Arul | 28 | 36000 |
