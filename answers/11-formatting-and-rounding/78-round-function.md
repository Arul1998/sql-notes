# Lesson 78 Answer: ROUND Function

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Round `Amount` to one decimal place.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 125.456 |
| 102 | 2 | 250.123 |
| 103 | 1 | 399.999 |

## Answer

```sql
SELECT OrderId,
       Amount,
       ROUND(Amount, 1) AS RoundedAmount
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | RoundedAmount |
|---:|---:|---:|
| 101 | 125.456 | 125.500 |
| 102 | 250.123 | 250.100 |
| 103 | 399.999 | 400.000 |
