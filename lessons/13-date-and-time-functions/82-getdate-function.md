# Lesson 82: GETDATE Function

`GETDATE` returns the current date and time from SQL Server.

## Sample Table

Imagine this `Employees` table:

| EmployeeId | EmployeeName |
|---:|---|
| 1 | Alice |
| 2 | Bob |
| 3 | Carol |

## Syntax

```sql
GETDATE()
```

## Example

```sql
SELECT GETDATE() AS CurrentDateTime;
```

## Exercise

Display `EmployeeId`, `EmployeeName`, and the current date and time.

Name the new column `CurrentDateTime`.
