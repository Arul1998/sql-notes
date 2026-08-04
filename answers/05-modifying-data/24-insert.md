# Lesson 24 Answer: INSERT

## Exercise

Insert a new order with `OrderId` 105, `CustomerId` 4, and `Amount` 250.

## Sample Table

### Orders Before INSERT

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |

## Answer

```sql
INSERT INTO Orders (OrderId, CustomerId, Amount)
VALUES (105, 4, 250);
```

## Expected Result

### Orders After INSERT

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |
