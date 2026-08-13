# Lesson 90 Answer: YEAR Function

## Exercise

Display `EmployeeId`, `HireDate`, and the year from `HireDate` as `HireYear`.

## Sample Table

| EmployeeId | HireDate |
|---:|---|
| 1 | 2024-06-15 |
| 2 | 2025-01-10 |

## Answer

```sql
SELECT EmployeeId, HireDate,
       YEAR(HireDate) AS HireYear
FROM Employees;
```

## Expected Result

| EmployeeId | HireDate | HireYear |
|---:|---|---:|
| 1 | 2024-06-15 | 2024 |
| 2 | 2025-01-10 | 2025 |
