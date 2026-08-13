# Lesson 88 Answer: EOMONTH Function

## Exercise

Display `OrderId`, `OrderDate`, and the last day of the month as `LastDayOfMonth`.

## Sample Table

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-10 |
| 102 | 2026-02-10 |

## Answer

```sql
SELECT OrderId, OrderDate,
       EOMONTH(OrderDate) AS LastDayOfMonth
FROM Orders;
```

## Expected Result

| OrderId | OrderDate | LastDayOfMonth |
|---:|---|---|
| 101 | 2026-08-10 | 2026-08-31 |
| 102 | 2026-02-10 | 2026-02-28 |
