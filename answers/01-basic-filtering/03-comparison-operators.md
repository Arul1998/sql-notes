# Lesson 3 Answer: Comparison Operators

## Exercise

Display `EmployeeName` and `Salary` for employees earning at least £40,000.

## Sample Table

### Employees

| EmployeeId | EmployeeName | Age | Salary |
|---:|---|---:|---:|
| 1 | Arul | 28 | 36000 |
| 2 | Priya | 32 | 45000 |
| 3 | John | 25 | 30000 |
| 4 | Sara | 35 | 52000 |
| 5 | Adam | 29 | 34000 |

## Answer

```sql
SELECT EmployeeName, Salary
FROM Employees
WHERE Salary >= 40000;
```

## Expected Result

| EmployeeName | Salary |
|---|---:|
| Priya | 45000 |
| Sara | 52000 |
