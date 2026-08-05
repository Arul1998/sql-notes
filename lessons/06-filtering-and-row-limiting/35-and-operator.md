# Lesson 35: Filtering with AND

`AND` returns a row only when every connected condition is true.

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
WHERE condition1 AND condition2;
```

## Example

```sql
SELECT *
FROM Employees
WHERE Department = 'IT' AND Salary > 30000;
```

Both the department and salary conditions must match.

## Exercise

Display employees in the `HR` department whose salary is greater than 40000.