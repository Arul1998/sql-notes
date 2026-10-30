# Lesson 124 Answer: COALESCE

## Exercise

Return EmployeeId and PreferredEmail. Use WorkEmail, then PersonalEmail, then 'No Email'.

## Sample Table

| EmployeeId | WorkEmail | PersonalEmail |
|---:|---|---|
| 1 | john@company.com | john@gmail.com |
| 2 | NULL | sarah@gmail.com |
| 3 | NULL | NULL |

## Answer

```sql
SELECT EmployeeId, COALESCE(WorkEmail, PersonalEmail, 'No Email') AS PreferredEmail
FROM Employees;
```

## Expected Result

| EmployeeId | PreferredEmail |
|---:|---|
| 1 | john@company.com |
| 2 | sarah@gmail.com |
| 3 | No Email |
