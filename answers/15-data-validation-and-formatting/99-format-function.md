# Lesson 99 Answer: FORMAT Function

## Exercise

Display `OrderId`, `OrderDate`, and format `OrderDate` as `dd/MM/yyyy` in `FormattedOrderDate`.

## Sample Table

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-12 |
| 102 | 2026-12-25 |

## Answer

```sql
SELECT OrderId, OrderDate,
       FORMAT(OrderDate, 'dd/MM/yyyy') AS FormattedOrderDate
FROM Orders;
```

## Expected Result

| OrderId | OrderDate | FormattedOrderDate |
|---:|---|---|
| 101 | 2026-08-12 | 12/08/2026 |
| 102 | 2026-12-25 | 25/12/2026 |
