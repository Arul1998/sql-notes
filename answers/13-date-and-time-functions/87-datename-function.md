# Lesson 87 Answer: DATENAME Function

## Exercise

Display `OrderId`, `OrderDate`, and the weekday name from `OrderDate` as `OrderDay`.

## Sample Table

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-10 |
| 102 | 2026-08-11 |

## Answer

```sql
SELECT OrderId, OrderDate,
       DATENAME(WEEKDAY, OrderDate) AS OrderDay
FROM Orders;
```

## Expected Result

| OrderId | OrderDate | OrderDay |
|---:|---|---|
| 101 | 2026-08-10 | Monday |
| 102 | 2026-08-11 | Tuesday |
