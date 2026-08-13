# Lesson 77: FLOOR Function

`FLOOR` rounds a number down to the nearest whole number.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 125.20 |
| 102 | 2 | 250.75 |
| 103 | 1 | 399.90 |

## Syntax

```sql
FLOOR(number)
```

## Example

```sql
SELECT OrderId,
       Amount,
       FLOOR(Amount) AS RoundedDownAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Use `FLOOR` to round `Amount` down to the nearest whole number.
