# Lesson 79 Answer: ABS Function

## Exercise

Display `OrderId`, `Amount`, and `PositiveAmount`.

Use `ABS` to return the absolute value of `Amount`.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | -500.00 |
| 102 | 250.00 |
| 103 | -100.00 |

## Answer

```sql
SELECT OrderId,
       Amount,
       ABS(Amount) AS PositiveAmount
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | PositiveAmount |
|---:|---:|---:|
| 101 | -500.00 | 500.00 |
| 102 | 250.00 | 250.00 |
| 103 | -100.00 | 100.00 |
