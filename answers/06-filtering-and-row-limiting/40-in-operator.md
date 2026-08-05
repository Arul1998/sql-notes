# Lesson 40 Answer: Filtering with IN

## Exercise

Display employees in the `IT` or `Finance` departments.

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
WHERE Department IN ('IT', 'Finance');
```

## Expected Result

### Result

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | Arul | IT | 36000 |
| 3 | John | IT | 30000 |
| 4 | Sara | Finance | 52000 |