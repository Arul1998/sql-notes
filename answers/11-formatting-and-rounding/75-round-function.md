# Lesson 75 Answer: ROUND Function

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Round `Amount` to one decimal place.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200.25 |
| 102 | 2 | 500.00 |
| 103 | 1 | 150.75 |
| 104 | 3 | 750.68 |
| 105 | 4 | 300.40 |

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
| 101 | 200.25 | 200.30 |
| 102 | 500.00 | 500.00 |
| 103 | 150.75 | 150.80 |
| 104 | 750.68 | 750.70 |
| 105 | 300.40 | 300.40 |
