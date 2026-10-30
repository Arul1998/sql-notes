# Lesson 103: ANY

`ANY` compares a value with at least one value returned by a subquery.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | John | IT | 40000 |
| 2 | Sarah | Sales | 50000 |
| 3 | David | IT | 30000 |

## Syntax

```sql
SELECT columns FROM table WHERE value > ANY (SELECT value FROM other_table);
```

## Example

```sql
SELECT EmployeeId, EmployeeName, Salary
FROM Employees
WHERE Salary > ANY (SELECT Salary
FROM Employees
WHERE Department = 'Sales');
```

## Exercise

Display employees whose salary is greater than at least one salary in the Sales department.
