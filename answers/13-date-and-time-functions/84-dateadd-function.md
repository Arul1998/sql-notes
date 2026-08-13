# Lesson 84 Answer: DATEADD Function

## Exercise

Display `OrderId`, `OrderDate`, and `ExpectedDate`.

Add 5 days to `OrderDate` using `DATEADD`.

## Sample Table

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-01 |
| 102 | 2026-08-05 |
| 103 | 2026-08-10 |

## Answer

```sql
SELECT OrderId,
       OrderDate,
       DATEADD(DAY, 5, OrderDate) AS ExpectedDate
FROM Orders;
```

## Expected Result

| OrderId | OrderDate | ExpectedDate |
|---:|---|---|
| 101 | 2026-08-01 | 2026-08-06 |
| 102 | 2026-08-05 | 2026-08-10 |
| 103 | 2026-08-10 | 2026-08-15 |
