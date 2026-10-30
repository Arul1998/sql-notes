# Lesson 124: COALESCE

`COALESCE` returns the first non-NULL value.

## Sample Table

| EmployeeId | WorkEmail | PersonalEmail |
|---:|---|---|
| 1 | john@company.com | john@gmail.com |
| 2 | NULL | sarah@gmail.com |
| 3 | NULL | NULL |

## Syntax

```sql
COALESCE(value1, value2, value3)
```

## Example

```sql
SELECT EmployeeId, COALESCE(WorkEmail, PersonalEmail, 'No Email') AS PreferredEmail
FROM Employees;
```

## Exercise

Return EmployeeId and PreferredEmail. Use WorkEmail, then PersonalEmail, then 'No Email'.
