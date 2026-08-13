# Lesson 94 Answer: CONVERT Function

## Exercise

Display `OrderId`, `Amount`, and convert `Amount` to `INT` as `WholeAmount`.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | 125.75 |
| 102 | 250.20 |

## Answer

```sql
SELECT OrderId, Amount,
       CONVERT(INT, Amount) AS WholeAmount
FROM Orders;
```

## Expected Result

| OrderId | Amount | WholeAmount |
|---:|---:|---:|
| 101 | 125.75 | 125 |
| 102 | 250.20 | 250 |
