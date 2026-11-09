# Lesson 134 Answer: LEFT

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `ProductPrefix`. Use `LEFT()` to extract the first three characters of each `ProductCode`.

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
    LEFT(ProductCode, 3) AS ProductPrefix
FROM Products;
```

## Expected Result

| ProductId | ProductName | ProductPrefix |
|---:|---|---|
| 1 | Laptop | LAP |
| 2 | Mouse | MOU |
| 3 | Keyboard | KEY |
| 4 | Monitor | MON |
