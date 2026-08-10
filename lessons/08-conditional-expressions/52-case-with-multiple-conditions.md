# Lesson 52: CASE with Multiple Conditions

A `CASE` expression can check multiple conditions.

SQL Server checks them from top to bottom and returns the first matching result.

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
CASE
    WHEN condition1 THEN result1
    WHEN condition2 THEN result2
    ELSE result3
END
```

## Example

```sql
SELECT OrderId,
       CASE
           WHEN Amount >= 600 THEN 'High'
           WHEN Amount >= 300 THEN 'Medium'
           ELSE 'Low'
       END AS AmountLevel
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `OrderSize` from `Orders`.

- `Amount >= 500` becomes `Large`.
- `Amount >= 200` becomes `Medium`.
- Otherwise, display `Small`.
