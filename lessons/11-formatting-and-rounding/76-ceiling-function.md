# Lesson 76: CEILING Function

`CEILING` rounds a number up to the next whole number.

Even if the decimal part is small, the number is rounded upward.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 125.20 |
| 102 | 2 | 250.75 |
| 103 | 1 | 399.10 |

## Syntax

```sql
CEILING(number)
```

## Example

```sql
SELECT OrderId,
       Amount,
       CEILING(Amount) AS RoundedUpAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Use `CEILING` to round `Amount` up to the next whole number.
