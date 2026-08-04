# Lesson 4 Answer: AND

## Exercise

Display `EmployeeName`, `Age`, and `Salary` for employees aged at least 30 and earning more than £40,000.

## Sample Table

### Employees

| EmployeeId | EmployeeName | Department | Age | Salary |
|---:|---|---|---:|---:|
| 1 | Arul | IT | 28 | 36000 |
| 2 | Priya | Finance | 32 | 45000 |
| 3 | John | IT | 25 | 30000 |
| 4 | Sara | Finance | 35 | 52000 |
| 5 | Adam | Sales | 29 | 34000 |

## Answer

```sql
SELECT EmployeeName, Age, Salary
FROM Employees
WHERE Age >= 30
  AND Salary > 40000;
```

## Expected Result

| EmployeeName | Age | Salary |
|---|---:|---:|
| Priya | 32 | 45000 |
| Sara | 35 | 52000 |
