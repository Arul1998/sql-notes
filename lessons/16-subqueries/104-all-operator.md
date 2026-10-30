# Lesson 104: ALL

`ALL` requires the comparison to be true for every value in the subquery.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | John | IT | 40000 |
| 2 | Sarah | Sales | 50000 |
| 3 | David | IT | 30000 |

## Syntax

```sql
SELECT columns FROM table WHERE value > ALL (SELECT value FROM other_table);
```

## Example

```sql
SELECT EmployeeId, EmployeeName, Salary
FROM Employees
WHERE Salary > ALL (SELECT Salary
FROM Employees
WHERE Department = 'IT');
```

## Exercise

Display employees earning more than every employee in the IT department.
