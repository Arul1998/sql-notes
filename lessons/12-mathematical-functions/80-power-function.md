# Lesson 80: POWER Function

`POWER` raises a number to a specified power.

## Sample Table

Imagine this `Orders` table:

| OrderId | Amount |
|---:|---:|
| 101 | 2 |
| 102 | 3 |
| 103 | 5 |

## Syntax

```sql
POWER(number, power)
```

## Example

```sql
SELECT OrderId,
       Amount,
       POWER(Amount, 2) AS AmountSquared
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `AmountSquared`.

Use `POWER` to calculate `Amount` to the power of 2.
