# Lesson 92: DAY Function

`DAY` extracts the day number of the month from a date.

## Sample Table

Imagine this `Employees` table:

| EmployeeId | HireDate |
|---:|---|
| 1 | 2024-06-15 |
| 2 | 2025-01-10 |

## Syntax

```sql
DAY(date)
```

## Example

```sql
SELECT EmployeeId,
       DAY(HireDate) AS HireDay
FROM Employees;
```

## Exercise

Display `EmployeeId`, `HireDate`, and the day from `HireDate`.

Name the new column `HireDay`.
