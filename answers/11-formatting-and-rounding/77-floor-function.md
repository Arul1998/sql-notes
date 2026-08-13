# Lesson 77 Answer: FLOOR Function

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Use `FLOOR` to round `Amount` down to the nearest whole number.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 125.20 |
| 102 | 2 | 250.75 |
| 103 | 1 | 399.90 |

## Answer

```sql
SELECT OrderId,
       Amount,
       FLOOR(Amount) AS RoundedAmount
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | RoundedAmount |
|---:|---:|---:|
| 101 | 125.20 | 125 |
| 102 | 250.75 | 250 |
| 103 | 399.90 | 399 |
