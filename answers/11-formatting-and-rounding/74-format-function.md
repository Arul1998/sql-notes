# Lesson 74 Answer: FORMAT Function

## Exercise

Display `OrderId`, `Amount`, and `FormattedAmount`.

Use `FORMAT` with `N2` to show two decimal places.

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
       FORMAT(Amount, 'N2') AS FormattedAmount
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | FormattedAmount |
|---:|---:|---:|
| 101 | 200.25 | 200.25 |
| 102 | 500.00 | 500.00 |
| 103 | 150.75 | 150.75 |
| 104 | 750.68 | 750.68 |
| 105 | 300.40 | 300.40 |
