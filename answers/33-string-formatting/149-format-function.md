# Lesson 149 Answer: FORMAT

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `FormattedPrice`. Use `FORMAT()` to show `Price` in British pounds with exactly two decimal places (`'C2'`, `'en-GB'`).

## Sample Table

| ProductId | ProductName | Price |
|---:|---|---:|
| 1 | Laptop | 1299.5 |
| 2 | Mouse | 25 |
| 3 | Keyboard | 79.99 |
| 4 | Monitor | 350.75 |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    FORMAT(Price, 'C2', 'en-GB') AS FormattedPrice
FROM Products;
```

## Expected Result

| ProductId | ProductName | FormattedPrice |
|---:|---|---|
| 1 | Laptop | £1,299.50 |
| 2 | Mouse | £25.00 |
| 3 | Keyboard | £79.99 |
| 4 | Monitor | £350.75 |
