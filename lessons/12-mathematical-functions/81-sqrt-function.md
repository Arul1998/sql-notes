# Lesson 81: SQRT Function

`SQRT` returns the square root of a number.

## Sample Table

Imagine this `Orders` table:

| OrderId | Amount |
|---:|---:|
| 101 | 25 |
| 102 | 64 |
| 103 | 100 |

## Syntax

```sql
SQRT(number)
```

## Example

```sql
SELECT OrderId,
       Amount,
       SQRT(Amount) AS AmountSquareRoot
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `SquareRootAmount`.

Use `SQRT` to calculate the square root of `Amount`.
