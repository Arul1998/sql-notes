# Lesson 8 Answer: BETWEEN

## Exercise

Display `EmployeeName` and `Age` for employees aged from 28 through 35. Sort the results from oldest to youngest.

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
SELECT EmployeeName, Age
FROM Employees
WHERE Age BETWEEN 28 AND 35
ORDER BY Age DESC;
```

## Expected Result

| EmployeeName | Age |
|---|---:|
| Sara | 35 |
| Priya | 32 |
| Adam | 29 |
| Arul | 28 |
