# Lesson 133 Answer: PATINDEX

## Exercise

Using `Products`, display `ProductId`, `ProductCode`, and `FirstNumberPosition`. Use `PATINDEX()` to find the position of the first digit (`0`–`9`) in each `ProductCode`.

## Sample Table

| ProductId | ProductCode |
|---:|---|
| 1 | LAP1001 |
| 2 | MOUSE202 |
| 3 | KEY45 |
| 4 | MONITOR789 |

## Answer

```sql
SELECT
    ProductId,
    ProductCode,
    PATINDEX('%[0-9]%', ProductCode) AS FirstNumberPosition
FROM Products;
```

## Expected Result

| ProductId | ProductCode | FirstNumberPosition |
|---:|---|---:|
| 1 | LAP1001 | 4 |
| 2 | MOUSE202 | 6 |
| 3 | KEY45 | 4 |
| 4 | MONITOR789 | 8 |
