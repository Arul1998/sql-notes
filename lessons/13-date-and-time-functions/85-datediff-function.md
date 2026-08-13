# Lesson 85: DATEDIFF Function

`DATEDIFF` calculates the difference between two dates using a chosen date part.

## Sample Table

Imagine this `Orders` table:

| OrderId | OrderDate | DeliveryDate |
|---:|---|---|
| 101 | 2026-08-01 | 2026-08-05 |
| 102 | 2026-08-03 | 2026-08-10 |
| 103 | 2026-08-10 | 2026-08-12 |

## Syntax

```sql
DATEDIFF(datepart, start_date, end_date)
```

## Example

```sql
SELECT OrderId,
       DATEDIFF(DAY, OrderDate, DeliveryDate) AS DeliveryDays
FROM Orders;
```

## Exercise

Display `OrderId`, `OrderDate`, `DeliveryDate`, and `DaysTaken`.

Find the difference in days between `OrderDate` and `DeliveryDate`.
