# Lesson 107: UPDATE with Subquery

A subquery can identify which rows to update.

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

## Syntax

```sql
UPDATE table SET column = value WHERE column IN (SELECT column FROM other_table WHERE condition);
```

## Example

```sql
UPDATE Employees SET Salary = Salary + 1000
WHERE Department IN (SELECT DepartmentName
FROM Departments
WHERE DepartmentName = 'IT');
```

## Exercise

Increase salaries by 1000 for employees in departments listed in Departments where DepartmentName is IT.
