# Lesson 12 Answer: TOP

## Exercise

Display the three youngest employees. Include `EmployeeName` and `Age`, and use SQL Server syntax.

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
SELECT TOP (3) EmployeeName, Age
FROM Employees
ORDER BY Age ASC;
```

## Expected Result

| EmployeeName | Age |
|---|---:|
| John | 25 |
| Arul | 28 |
| Adam | 29 |
