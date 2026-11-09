# Lesson 131 Answer: STUFF

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `UpdatedProductCode`. Replace the first three characters (`PRD`) of each `ProductCode` with `ITEM`, preserving the hyphen.

## Sample Table

| ProductId | ProductName | ProductCode |
|---:|---|---|
| 1 | Laptop | PRD-1001 |
| 2 | Mouse | PRD-1002 |
| 3 | Keyboard | PRD-1003 |
| 4 | Monitor | PRD-1004 |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    STUFF(ProductCode, 1, 3, 'ITEM') AS UpdatedProductCode
FROM Products;
```

## Expected Result

| ProductId | ProductName | UpdatedProductCode |
|---:|---|---|
| 1 | Laptop | ITEM-1001 |
| 2 | Mouse | ITEM-1002 |
| 3 | Keyboard | ITEM-1003 |
| 4 | Monitor | ITEM-1004 |
