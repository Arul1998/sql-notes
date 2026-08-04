# Lesson 11 Answer: NULL Values

## Exercise

Display `EmployeeName`, `Department`, and `Salary` for employees whose department is not missing. Sort them from the lowest salary to the highest.

## Sample Table

### Employees

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| John | NULL | 30000 |
| Sara | Finance | 52000 |

## Answer

```sql
SELECT EmployeeName, Department, Salary
FROM Employees
WHERE Department IS NOT NULL
ORDER BY Salary ASC;
```

## Expected Result

| EmployeeName | Department | Salary |
|---|---|---:|
| Arul | IT | 36000 |
| Priya | Finance | 45000 |
| Sara | Finance | 52000 |
