# Lesson 136 Answer: SUBSTRING

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `CategoryCode`. Use `SUBSTRING()` to extract the three-letter category code at position 5 in each `ProductCode`.

## Sample Table

| ProductId | ProductName | ProductCode |
|---:|---|---|
| 1 | Laptop | PRD-LAP-1001 |
| 2 | Mouse | PRD-MOU-2002 |
| 3 | Keyboard | PRD-KEY-3003 |
| 4 | Monitor | PRD-MON-4004 |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    SUBSTRING(ProductCode, 5, 3) AS CategoryCode
FROM Products;
```

## Expected Result

| ProductId | ProductName | CategoryCode |
|---:|---|---|
| 1 | Laptop | LAP |
| 2 | Mouse | MOU |
| 3 | Keyboard | KEY |
| 4 | Monitor | MON |
