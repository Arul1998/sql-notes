# Lesson 36: Filtering with OR

`OR` returns a row when at least one connected condition is true.

## Sample Table

| EmployeeId | EmployeeName | Department | Salary |
|---:|---|---|---:|
| 1 | Arul | IT | 36000 |
| 2 | Priya | HR | 45000 |
| 3 | John | IT | 30000 |
| 4 | Sara | Finance | 52000 |
| 5 | Adam | Sales | 34000 |
| 6 | Maya | NULL | 41000 |

## Syntax

```sql
SELECT columns
FROM table_name
WHERE condition1 OR condition2;
```

## Example

```sql
SELECT *
FROM Employees
WHERE Department = 'HR' OR Salary > 50000;
```

A row does not need to satisfy both conditions.

## Exercise

Display employees who work in `Sales` or earn more than 50000.