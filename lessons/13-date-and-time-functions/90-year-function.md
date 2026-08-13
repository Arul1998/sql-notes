# Lesson 90: YEAR Function

`YEAR` extracts the year from a date.

## Sample Table

Imagine this `Employees` table:

| EmployeeId | HireDate |
|---:|---|
| 1 | 2024-06-15 |
| 2 | 2025-01-10 |

## Syntax

```sql
YEAR(date)
```

## Example

```sql
SELECT EmployeeId,
       YEAR(HireDate) AS HireYear
FROM Employees;
```

## Exercise

Display `EmployeeId`, `HireDate`, and the year from `HireDate`.

Name the new column `HireYear`.
