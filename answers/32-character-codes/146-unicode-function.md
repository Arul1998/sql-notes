# Lesson 146 Answer: UNICODE

## Exercise

Using `Customers`, display `CustomerId`, `CustomerName`, and `FirstCharacterUnicode`. Use `UNICODE()` to find the Unicode value of the first character of each `CustomerName`.

## Sample Table

`CustomerName` is `NVARCHAR(100)`.

| CustomerId | CustomerName |
|---:|---|
| 1 | Alice |
| 2 | Bob |
| 3 | Charlie |
| 4 | David |

## Answer

```sql
SELECT
    CustomerId,
    CustomerName,
    UNICODE(CustomerName) AS FirstCharacterUnicode
FROM Customers;
```

## Expected Result

| CustomerId | CustomerName | FirstCharacterUnicode |
|---:|---|---:|
| 1 | Alice | 65 |
| 2 | Bob | 66 |
| 3 | Charlie | 67 |
| 4 | David | 68 |
