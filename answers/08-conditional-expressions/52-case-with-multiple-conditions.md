# Lesson 52 Answer: CASE with Multiple Conditions

## Exercise

Display `OrderId`, `Amount`, and `OrderSize` from `Orders`.

- `Amount >= 500` becomes `Large`.
- `Amount >= 200` becomes `Medium`.
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
           WHEN Amount >= 200 THEN 'Medium'
           ELSE 'Small'
       END AS OrderSize
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | OrderSize |
|---:|---:|---|
| 101 | 200 | Medium |
| 102 | 500 | Large |
| 103 | 150 | Small |
| 104 | 750 | Large |
| 105 | 300 | Medium |
