# Lesson 91: MONTH Function

`MONTH` extracts the month number from a date.

## Sample Table

Imagine this `Employees` table:

| EmployeeId | HireDate |
|---:|---|
| 1 | 2024-06-15 |
| 2 | 2025-01-10 |

## Syntax

```sql
MONTH(date)
```

## Example

```sql
SELECT EmployeeId,
       MONTH(HireDate) AS HireMonth
FROM Employees;
```

## Exercise

Display `EmployeeId`, `HireDate`, and the month from `HireDate`.

Name the new column `HireMonth`.
