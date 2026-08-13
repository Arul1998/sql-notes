# Lesson 78: ROUND Function

`ROUND` rounds a number to a specified number of decimal places.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 125.456 |
| 102 | 2 | 250.123 |
| 103 | 1 | 399.999 |

## Syntax

```sql
ROUND(number, decimal_places)
```

## Example

```sql
SELECT OrderId,
       Amount,
       ROUND(Amount, 2) AS RoundedAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Round `Amount` to one decimal place.
