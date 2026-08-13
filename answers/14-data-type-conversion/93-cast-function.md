# Lesson 93 Answer: CAST Function

## Exercise

Display `OrderId`, `Amount`, and convert `Amount` to `INT` as `IntegerAmount`.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | 125.75 |
| 102 | 250.20 |

## Answer

```sql
SELECT OrderId, Amount,
       CAST(Amount AS INT) AS IntegerAmount
FROM Orders;
```

## Expected Result

| OrderId | Amount | IntegerAmount |
|---:|---:|---:|
| 101 | 125.75 | 125 |
| 102 | 250.20 | 250 |
