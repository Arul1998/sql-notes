# Lesson 132 Answer: CHARINDEX

## Exercise

Using `Products`, display `ProductId`, `ProductCode`, and `HyphenPosition`. Use `CHARINDEX()` to find the position of `-` in each `ProductCode`.

## Sample Table

| ProductId | ProductCode |
|---:|---|
| 1 | LAP-1001 |
| 2 | MOU-2002 |
| 3 | KEY-3003 |
| 4 | MON-4004 |

## Answer

```sql
SELECT
    ProductId,
    ProductCode,
    CHARINDEX('-', ProductCode) AS HyphenPosition
FROM Products;
```

## Expected Result

| ProductId | ProductCode | HyphenPosition |
|---:|---|---:|
| 1 | LAP-1001 | 4 |
| 2 | MOU-2002 | 4 |
| 3 | KEY-3003 | 4 |
| 4 | MON-4004 | 4 |
