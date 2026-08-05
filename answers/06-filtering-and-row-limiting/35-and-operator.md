# Lesson 35 Answer: Filtering with AND

## Exercise

Display employees in the `HR` department whose salary is greater than 40000.

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
WHERE Department = 'HR' AND Salary > 40000;
```

## Expected Result

### Result

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 2 | Priya | HR | 45000 |