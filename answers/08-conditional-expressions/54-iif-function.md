# Lesson 54 Answer: IIF Function

## Exercise

Display `OrderId`, `Amount`, and `OrderStatus` from `Orders`.

If `Amount` is 300 or more, display `Priority`. Otherwise, display `Normal`.

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
       IIF(Amount >= 300, 'Priority', 'Normal') AS OrderStatus
FROM Orders;
```

## Expected Result

### Result

| OrderId | Amount | OrderStatus |
|---:|---:|---|
| 101 | 200 | Normal |
| 102 | 500 | Priority |
| 103 | 150 | Normal |
| 104 | 750 | Priority |
| 105 | 300 | Priority |
