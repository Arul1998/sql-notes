# Lesson 128 Answer: REPLACE

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `UpdatedCategory`. Use `REPLACE()` to display `Smartphone` instead of `Mobile` in `Category`, without updating the table.

## Sample Table

| ProductId | ProductName | Category |
|---:|---|---|
| 1 | Apple iPhone | Mobile |
| 2 | Samsung Galaxy | Mobile |
| 3 | Dell Laptop | Computer |
| 4 | HP Laptop | Computer |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    REPLACE(Category, 'Mobile', 'Smartphone') AS UpdatedCategory
FROM Products;
```

## Expected Result

| ProductId | ProductName | UpdatedCategory |
|---:|---|---|
| 1 | Apple iPhone | Smartphone |
| 2 | Samsung Galaxy | Smartphone |
| 3 | Dell Laptop | Computer |
| 4 | HP Laptop | Computer |
