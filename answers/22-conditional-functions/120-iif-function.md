# Lesson 120 Answer: IIF

## Exercise

Display EmployeeName and SalaryLevel ('High' for Salary at least 40000, otherwise 'Low').

## Sample Table

| EmployeeName | Salary |
|---|---:|
| John | 40000 |
| Sarah | 50000 |
| David | 30000 |

## Answer

```sql
SELECT EmployeeName, IIF(Salary >= 40000, 'High', 'Low') AS SalaryLevel
FROM Employees;
```

## Expected Result

| EmployeeName | SalaryLevel |
|---|---|
| John | High |
| Sarah | High |
| David | Low |
