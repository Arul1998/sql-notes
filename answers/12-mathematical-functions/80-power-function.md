# Lesson 80 Answer: POWER Function

## Exercise

Display `OrderId`, `Amount`, and `AmountSquared`.

Use `POWER` to calculate `Amount` to the power of 2.

## Sample Table

| OrderId | Amount |
|---:|---:|
| 101 | 2 |
| 102 | 3 |
| 103 | 5 |

## Answer

```sql
SELECT OrderId,
       Amount,
       POWER(Amount, 2) AS AmountSquared
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | AmountSquared |
|---:|---:|---:|
| 101 | 2 | 4 |
| 102 | 3 | 9 |
| 103 | 5 | 25 |
