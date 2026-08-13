# Lesson 82 Answer: GETDATE Function

## Exercise

Display `EmployeeId`, `EmployeeName`, and the current date and time.

Name the new column `CurrentDateTime`.

## Sample Table

| EmployeeId | EmployeeName |
|---:|---|
| 1 | Alice |
| 2 | Bob |
| 3 | Carol |

## Answer

```sql
SELECT EmployeeId,
       EmployeeName,
       GETDATE() AS CurrentDateTime
FROM Employees;
```

## Expected Result

### Result

| EmployeeId | EmployeeName | CurrentDateTime |
|---:|---|---|
| 1 | Alice | Current SQL Server date and time |
| 2 | Bob | Current SQL Server date and time |
| 3 | Carol | Current SQL Server date and time |
