# Lesson 123: ISNULL

`ISNULL` replaces NULL with a specified value.

## Sample Table

| OrderId | Discount |
|---:|---:|
| 101 | 10 |
| 102 | NULL |
| 103 | 25 |

## Syntax

```sql
ISNULL(expression, replacement_value)
```

## Example

```sql
SELECT OrderId, Discount, ISNULL(Discount, 0) AS FinalDiscount
FROM Orders;
```

## Exercise

Return OrderId, Discount and FinalDiscount. Replace NULL discounts with 0.
