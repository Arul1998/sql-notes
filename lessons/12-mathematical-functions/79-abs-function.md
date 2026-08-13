# Lesson 79: ABS Function

`ABS` returns the absolute value of a number.

Negative numbers become positive, while positive numbers stay positive.

## Sample Table

Imagine this `Orders` table:

| OrderId | Amount |
|---:|---:|
| 101 | -500.00 |
| 102 | 250.00 |
| 103 | -100.00 |

## Syntax

```sql
ABS(number)
```

## Example

```sql
SELECT OrderId,
       Amount,
       ABS(Amount) AS AbsoluteAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `PositiveAmount`.

Use `ABS` to return the absolute value of `Amount`.
