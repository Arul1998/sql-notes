# Lesson 76 Answer: CEILING Function

## Exercise

Display `OrderId`, `Amount`, and `RoundedAmount`.

Use `CEILING` to round `Amount` up to the next whole number.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 125.20 |
| 102 | 2 | 250.75 |
| 103 | 1 | 399.10 |

## Answer

```sql
SELECT OrderId,
       Amount,
       CEILING(Amount) AS RoundedAmount
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | RoundedAmount |
|---:|---:|---:|
| 101 | 125.20 | 126 |
| 102 | 250.75 | 251 |
| 103 | 399.10 | 400 |
