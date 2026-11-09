# Lesson 144 Answer: ASCII

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `FirstLetterASCII`. Use `ASCII()` to find the numeric value of the first character of each `ProductName`.

## Sample Table

| ProductId | ProductName |
|---:|---|
| 1 | Laptop |
| 2 | Mouse |
| 3 | Keyboard |
| 4 | Monitor |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    ASCII(ProductName) AS FirstLetterASCII
FROM Products;
```

## Expected Result

| ProductId | ProductName | FirstLetterASCII |
|---:|---|---:|
| 1 | Laptop | 76 |
| 2 | Mouse | 77 |
| 3 | Keyboard | 75 |
| 4 | Monitor | 77 |
