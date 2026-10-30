# Lesson 104 Answer: ALL

## Exercise

Display employees earning more than every employee in the IT department.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | John | IT | 40000 |
| 2 | Sarah | Sales | 50000 |
| 3 | David | IT | 30000 |

## Answer

```sql
SELECT EmployeeId, EmployeeName, Salary
FROM Employees
WHERE Salary > ALL (SELECT Salary
FROM Employees
WHERE Department = 'IT');
```

## Expected Result

| EmployeeId | EmployeeName | Salary |
|---:|---|---:|
| 2 | Sarah | 50000 |
