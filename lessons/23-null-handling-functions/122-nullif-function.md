# Lesson 122: NULLIF

`NULLIF` returns NULL when two expressions are equal. Otherwise, it returns the first expression.

## Sample Table

| OrderId | Discount |
|---:|---:|
| 101 | 10 |
| 102 | 0 |
| 103 | 25 |

## Syntax

```sql
NULLIF(expression1, expression2)
```

## Example

```sql
SELECT OrderId, Discount, NULLIF(Discount, 0) AS ValidDiscount
FROM Orders;
```

## Exercise

Return OrderId, Discount and ValidDiscount. Replace zero discounts with NULL using NULLIF.
