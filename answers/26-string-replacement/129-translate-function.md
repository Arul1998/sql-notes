# Lesson 129 Answer: TRANSLATE

## Exercise

Using `Employees`, display `EmployeeId` and `UpdatedEmployeeCode`. Replace each hyphen (`-`) in `EmployeeCode` with `_` and each slash (`/`) with `#` using `TRANSLATE()`.

## Sample Table

| EmployeeId | EmployeeCode |
|---:|---|
| 1 | EMP-101/IT |
| 2 | EMP/202-HR |
| 3 | EMP-303/FIN |

## Answer

```sql
SELECT
    EmployeeId,
    TRANSLATE(EmployeeCode, '-/', '_#') AS UpdatedEmployeeCode
FROM Employees;
```

## Expected Result

| EmployeeId | UpdatedEmployeeCode |
|---:|---|
| 1 | EMP_101#IT |
| 2 | EMP#202_HR |
| 3 | EMP_303#FIN |
