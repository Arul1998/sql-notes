# Lesson 81 Answer: SQRT Function

## Exercise

Display `OrderId`, `Amount`, and `SquareRootAmount`.

Use `SQRT` to calculate the square root of `Amount`.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | 25 |
| 102 | 64 |
| 103 | 100 |

## Answer

```sql
SELECT OrderId,
       Amount,
       SQRT(Amount) AS SquareRootAmount
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | SquareRootAmount |
|---:|---:|---:|
| 101 | 25 | 5 |
| 102 | 64 | 8 |
| 103 | 100 | 10 |
