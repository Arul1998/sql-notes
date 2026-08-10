# Lesson 51 Answer: CASE Expression

## Exercise

Display `OrderId`, `Amount`, and a calculated column named `OrderSize` from the `Orders` table.

- If `Amount` is 500 or more, display `Large`.
- Otherwise, display `Small`.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 500 |
| 103 | 1 | 150 |
| 104 | 3 | 750 |
| 105 | 4 | 300 |

## Answer

```sql
SELECT OrderId,
       Amount,
       CASE
           WHEN Amount >= 500 THEN 'Large'
           ELSE 'Small'
       END AS OrderSize
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | OrderSize |
|---:|---:|---|
| 101 | 200 | Small |
| 102 | 500 | Large |
| 103 | 150 | Small |
| 104 | 750 | Large |
| 105 | 300 | Small |
