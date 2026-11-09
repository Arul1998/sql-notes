# Lesson 145 Answer: CHAR

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `CategoryLetter`. Convert the numeric `CategoryCode` values into characters using `CHAR()`.

## Sample Table

| ProductId | ProductName | CategoryCode |
|---:|---|---:|
| 1 | Laptop | 69 |
| 2 | Mouse | 77 |
| 3 | Keyboard | 75 |
| 4 | Monitor | 83 |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    CHAR(CategoryCode) AS CategoryLetter
FROM Products;
```

## Expected Result

| ProductId | ProductName | CategoryLetter |
|---:|---|---|
| 1 | Laptop | E |
| 2 | Mouse | M |
| 3 | Keyboard | K |
| 4 | Monitor | S |
