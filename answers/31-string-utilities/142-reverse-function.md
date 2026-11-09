# Lesson 142 Answer: REVERSE

## Exercise

Using `Products`, display `ProductId`, `ProductCode`, and `ReversedProductCode`. Use `REVERSE()` to reverse every character of `ProductCode`.

## Sample Table

| ProductId | ProductCode |
|---:|---|
| 1 | LAP100 |
| 2 | MOU200 |
| 3 | KEY300 |
| 4 | MON400 |

## Answer

```sql
SELECT
    ProductId,
    ProductCode,
    REVERSE(ProductCode) AS ReversedProductCode
FROM Products;
```

## Expected Result

| ProductId | ProductCode | ReversedProductCode |
|---:|---|---|
| 1 | LAP100 | 001PAL |
| 2 | MOU200 | 002UOM |
| 3 | KEY300 | 003YEK |
| 4 | MON400 | 004NOM |
