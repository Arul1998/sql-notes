# Lesson 75: ROUND Function

`ROUND` rounds a number to a specified number of decimal places.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200.25 |
| 102 | 2 | 500.00 |
| 103 | 1 | 150.75 |
| 104 | 3 | 750.68 |
| 105 | 4 | 300.40 |

## Syntax

```sql
ROUND(number, decimal_places)
```

## Example

```sql
SELECT OrderId,
       ROUND(Amount, 0) AS RoundedAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Round `Amount` to one decimal place.
