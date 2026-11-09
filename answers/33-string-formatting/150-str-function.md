# Lesson 150 Answer: STR

## Exercise

Using `Orders`, display `OrderId`, `CustomerName`, and `AmountText`. Use `STR(TotalAmount, 10, 2)` and `LTRIM()` to show each amount as text with two decimal places and no leading spaces.

## Sample Table

| OrderId | CustomerName | TotalAmount |
|---:|---|---:|
| 101 | Arun | 1500.456 |
| 102 | Priya | 250.5 |
| 103 | James | 75.999 |
| 104 | Sarah | 3200.125 |

## Answer

```sql
SELECT
    OrderId,
    CustomerName,
    LTRIM(STR(TotalAmount, 10, 2)) AS AmountText
FROM Orders;
```

## Expected Result

| OrderId | CustomerName | AmountText |
|---:|---|---|
| 101 | Arun | `1500.46` |
| 102 | Priya | `250.50` |
| 103 | James | `76.00` |
| 104 | Sarah | `3200.13` |
