# Lesson 41 Answer: Filtering with NOT IN

## Exercise

Display employees who are not in the `IT` or `HR` departments.

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
WHERE Department NOT IN ('IT', 'HR');
```

## Expected Result

### Result

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 4 | Sara | Finance | 52000 |
| 5 | Adam | Sales | 34000 |