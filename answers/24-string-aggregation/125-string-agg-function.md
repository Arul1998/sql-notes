# Lesson 125 Answer: STRING_AGG

## Exercise

Return CustomerId and Products. Combine product names for each customer using ', ' as the separator.

## Sample Table

| OrderId | CustomerId | ProductName |
|---:|---:|---|
| 101 | 1 | Laptop |
| 102 | 1 | Mouse |
| 103 | 2 | Keyboard |
| 104 | 2 | Monitor |

## Answer

```sql
SELECT CustomerId, STRING_AGG(ProductName, ', ') AS Products
FROM Orders
GROUP BY CustomerId;
```

## Expected Result

| CustomerId | Products |
|---:|---|
| 1 | Laptop, Mouse |
| 2 | Keyboard, Monitor |
