# Lesson 86 Answer: DATEPART Function

## Exercise

Display `OrderId`, `OrderDate`, and the year from `OrderDate` as `OrderYear`.

## Sample Table

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-10 |
| 102 | 2025-12-05 |

## Answer

```sql
SELECT OrderId, OrderDate,
       DATEPART(YEAR, OrderDate) AS OrderYear
FROM Orders;
```

## Expected Result

| OrderId | OrderDate | OrderYear |
|---:|---|---:|
| 101 | 2026-08-10 | 2026 |
| 102 | 2025-12-05 | 2025 |
