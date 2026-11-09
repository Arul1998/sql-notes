# Lesson 135 Answer: RIGHT

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `ProductNumber`. Use `RIGHT()` to extract the last four characters of each `ProductCode`.

## Sample Table

| ProductId | ProductName | ProductCode |
|---:|---|---|
| 1 | Laptop | LAP1001 |
| 2 | Mouse | MOU2002 |
| 3 | Keyboard | KEY3003 |
| 4 | Monitor | MON4004 |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    RIGHT(ProductCode, 4) AS ProductNumber
FROM Products;
```

## Expected Result

| ProductId | ProductName | ProductNumber |
|---:|---|---|
| 1 | Laptop | 1001 |
| 2 | Mouse | 2002 |
| 3 | Keyboard | 3003 |
| 4 | Monitor | 4004 |
