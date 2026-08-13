# Lesson 91 Answer: MONTH Function

## Exercise

Display `EmployeeId`, `HireDate`, and the month from `HireDate` as `HireMonth`.

## Sample Table

| EmployeeId | HireDate |
|---:|---|
| 1 | 2024-06-15 |
| 2 | 2025-01-10 |

## Answer

```sql
SELECT EmployeeId, HireDate,
       MONTH(HireDate) AS HireMonth
FROM Employees;
```

## Expected Result

| EmployeeId | HireDate | HireMonth |
|---:|---|---:|
| 1 | 2024-06-15 | 6 |
| 2 | 2025-01-10 | 1 |
