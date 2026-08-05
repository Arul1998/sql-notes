# Lesson 36 Answer: Filtering with OR

## Exercise

Display employees who work in `Sales` or earn more than 50000.

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
SELECT *
FROM Employees
WHERE Department = 'Sales' OR Salary > 50000;
```

## Expected Result

### Result

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 4 | Sara | Finance | 52000 |
| 5 | Adam | Sales | 34000 |