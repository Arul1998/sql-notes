# Lesson 58 Answer: NULLIF Function

## Exercise

Display `OrderId`, `Amount`, and `ValidAmount` from `Orders`.

Use `NULLIF` to return `NULL` when `Amount` is `0`. Otherwise, return the original amount.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 500 |
| 103 | 1 | 150 |
| 104 | 3 | 750 |
| 105 | 4 | 300 |

## Answer

```sql
SELECT OrderId,
       Amount,
       NULLIF(Amount, 0) AS ValidAmount
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | ValidAmount |
|---:|---:|---:|
| 101 | 200 | 200 |
| 102 | 500 | 500 |
| 103 | 150 | 150 |
| 104 | 750 | 750 |
| 105 | 300 | 300 |
