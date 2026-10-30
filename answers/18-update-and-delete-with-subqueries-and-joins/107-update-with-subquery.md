# Lesson 107 Answer: UPDATE with Subquery

## Exercise

Increase salaries by 1000 for employees in departments listed in Departments where DepartmentName is IT.

## Sample Tables

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | John | IT | 40000 |
| 2 | Sarah | Sales | 50000 |
| 3 | David | IT | 30000 |

**Departments**

| DepartmentName |
|---|
| IT |
| Sales |

## Answer

```sql
UPDATE Employees SET Salary = Salary + 1000
WHERE Department IN (SELECT DepartmentName
FROM Departments
WHERE DepartmentName = 'IT');
```

## Expected Result

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | John | IT | 41000 |
| 2 | Sarah | Sales | 50000 |
| 3 | David | IT | 31000 |
