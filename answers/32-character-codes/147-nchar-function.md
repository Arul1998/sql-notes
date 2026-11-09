# Lesson 147 Answer: NCHAR

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `UnicodeCharacter`. Convert each `UnicodeCode` into its corresponding character using `NCHAR()`.

## Sample Table

| ProductId | ProductName | UnicodeCode |
|---:|---|---:|
| 1 | Laptop | 65 |
| 2 | Mouse | 66 |
| 3 | Keyboard | 67 |
| 4 | Monitor | 2980 |

## Answer

```sql
SELECT
    ProductId,
    ProductName,
    NCHAR(UnicodeCode) AS UnicodeCharacter
FROM Products;
```

## Expected Result

| ProductId | ProductName | UnicodeCharacter |
|---:|---|---|
| 1 | Laptop | A |
| 2 | Mouse | B |
| 3 | Keyboard | C |
| 4 | Monitor | த |
