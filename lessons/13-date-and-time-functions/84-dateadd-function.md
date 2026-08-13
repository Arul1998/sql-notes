# Lesson 84: DATEADD Function

`DATEADD` adds or subtracts a specified amount of time from a date.

## Sample Table

Imagine this `Orders` table:

| OrderId | OrderDate |
|---:|---|
| 101 | 2026-08-01 |
| 102 | 2026-08-05 |
| 103 | 2026-08-10 |

## Syntax

```sql
DATEADD(datepart, number, date)
```

## Example

```sql
SELECT OrderId,
       OrderDate,
       DATEADD(DAY, 10, OrderDate) AS DeliveryDate
FROM Orders;
```

## Exercise

Display `OrderId`, `OrderDate`, and `ExpectedDate`.

Add 5 days to `OrderDate` using `DATEADD`.
