# Lesson 15 Answer: MIN and MAX

## Exercise

Find the youngest and oldest employee ages. Name the result columns `YoungestAge` and `OldestAge`.

## Sample Table

### Employees

| EmployeeName | Age | Salary |
|---|---:|---:|
| Arul | 28 | 36000 |
| Priya | 32 | 45000 |
| John | 25 | 30000 |
| Sara | 35 | 52000 |
| Adam | 29 | 34000 |

## Answer

```sql
SELECT
    MIN(Age) AS YoungestAge,
    MAX(Age) AS OldestAge
FROM Employees;
```

## Expected Result

| YoungestAge | OldestAge |
|---:|---:|
| 25 | 35 |
