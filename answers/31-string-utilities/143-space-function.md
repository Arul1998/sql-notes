# Lesson 143 Answer: SPACE

## Exercise

Using `Customers`, display `CustomerId` and `CustomerFullName`. Use `CONCAT()` and `SPACE(3)` to place exactly three spaces between each `FirstName` and `LastName`.

## Sample Table

| CustomerId | FirstName | LastName |
|---:|---|---|
| 1 | Arun | Kumar |
| 2 | Priya | Sharma |
| 3 | James | Brown |
| 4 | David | Wilson |

## Answer

```sql
SELECT
    CustomerId,
    CONCAT(FirstName, SPACE(3), LastName) AS CustomerFullName
FROM Customers;
```

## Expected Result

| CustomerId | CustomerFullName |
|---:|---|
| 1 | `Arun   Kumar` |
| 2 | `Priya   Sharma` |
| 3 | `James   Brown` |
| 4 | `David   Wilson` |
