# Lesson 130 Answer: REPLICATE

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `StockDisplay`. Use `REPLICATE()` to display one `#` for each unit in `StockLevel`.

## Sample Table

| ProductId | ProductName | StockLevel |
|---:|---|---:|
| 1 | Laptop | 4 |
| 2 | Mouse | 2 |
| 3 | Keyboard | 5 |
| 4 | Monitor | 3 |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    REPLICATE('#', StockLevel) AS StockDisplay
FROM Products;
```

## Expected Result

| ProductId | ProductName | StockDisplay |
|---:|---|---|
| 1 | Laptop | `####` |
| 2 | Mouse | `##` |
| 3 | Keyboard | `#####` |
| 4 | Monitor | `###` |
