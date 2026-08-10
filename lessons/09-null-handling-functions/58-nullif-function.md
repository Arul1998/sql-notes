# Lesson 58: NULLIF Function

`NULLIF` returns `NULL` when two values are equal. Otherwise, it returns the first value.

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
NULLIF(value1, value2)
```

## Example

```sql
SELECT OrderId,
       NULLIF(Amount, 200) AS CheckedAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `ValidAmount` from `Orders`.

Use `NULLIF` to return `NULL` when `Amount` is `0`. Otherwise, return the original amount.
