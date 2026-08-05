# Lesson 50: COUNT with an Alias

Use `AS` to give a calculated `COUNT` column a clear name.

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
SELECT COUNT(*) AS alias_name
FROM table_name;
```

## Example

```sql
SELECT COUNT(*) AS TotalEmployees
FROM Employees;
```

An alias makes the query result easier to understand.

## Exercise

Count all employees and name the result column `TotalEmployees`.