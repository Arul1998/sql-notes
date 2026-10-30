# Lesson 123 Answer: ISNULL

## Exercise

Return OrderId, Discount and FinalDiscount. Replace NULL discounts with 0.

## Sample Table

| OrderId | Discount |
|---:|---:|
| 101 | 10 |
| 102 | NULL |
| 103 | 25 |

## Answer

```sql
SELECT OrderId, Discount, ISNULL(Discount, 0) AS FinalDiscount
FROM Orders;
```

## Expected Result

| OrderId | Discount | FinalDiscount |
|---:|---:|---:|
| 101 | 10 | 10 |
| 102 | NULL | 0 |
| 103 | 25 | 25 |
