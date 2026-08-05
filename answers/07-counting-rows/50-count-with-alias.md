# Lesson 50 Answer: COUNT with an Alias

## Exercise

Count all employees and name the result column `TotalEmployees`.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | Arul | IT | 36000 |
| 2 | Priya | HR | 45000 |
| 3 | John | IT | 30000 |
| 4 | Sara | Finance | 52000 |
| 5 | Adam | Sales | 34000 |
| 6 | Maya | NULL | 41000 |

## Answer

```sql
SELECT COUNT(*) AS TotalEmployees
FROM Employees;
```

## Expected Result

### Result

| TotalEmployees |
|---:|
| 6 |