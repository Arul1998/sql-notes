# Lesson 54: IIF Function

`IIF` returns one value when a condition is true and another when it is false.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 500 |
| 103 | 1 | 150 |
| 104 | 3 | 750 |
| 105 | 4 | 300 |

## Syntax

```sql
IIF(condition, value_if_true, value_if_false)
```

## Example

```sql
SELECT OrderId,
       IIF(Amount >= 500, 'High', 'Standard') AS AmountLevel
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `OrderStatus` from `Orders`.

If `Amount` is 300 or more, display `Priority`. Otherwise, display `Normal`.
