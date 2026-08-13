# Lesson 92 Answer: DAY Function

## Exercise

Display `EmployeeId`, `HireDate`, and the day from `HireDate` as `HireDay`.

## Sample Table

| EmployeeId | HireDate |
|---:|---|
| 1 | 2024-06-15 |
| 2 | 2025-01-10 |

## Answer

```sql
SELECT EmployeeId, HireDate,
       DAY(HireDate) AS HireDay
FROM Employees;
```

## Expected Result

| EmployeeId | HireDate | HireDay |
|---:|---|---:|
| 1 | 2024-06-15 | 15 |
| 2 | 2025-01-10 | 10 |
