# Lesson 122 Answer: NULLIF

## Exercise

Return OrderId, Discount and ValidDiscount. Replace zero discounts with NULL using NULLIF.

## Sample Table

| OrderId | Discount |
|---:|---:|
| 101 | 10 |
| 102 | 0 |
| 103 | 25 |

## Answer

```sql
SELECT OrderId, Discount, NULLIF(Discount, 0) AS ValidDiscount
FROM Orders;
```

## Expected Result

| OrderId | Discount | ValidDiscount |
|---:|---:|---:|
| 101 | 10 | 10 |
| 102 | 0 | NULL |
| 103 | 25 | 25 |
