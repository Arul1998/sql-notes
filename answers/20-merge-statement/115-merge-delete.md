# Lesson 115 Answer: MERGE (DELETE Missing Rows)

## Exercise

Delete products that do not appear in NewProducts.

## Sample Tables

**Products**

| ProductId | ProductName |
|---:|---|
| 1 | Laptop |
| 2 | Mouse |
| 3 | Keyboard |

**NewProducts**

| ProductId | ProductName |
|---:|---|
| 1 | Laptop |
| 3 | Keyboard |

## Answer

```sql
MERGE Products AS t
USING NewProducts AS s ON t.ProductId = s.ProductId
WHEN NOT MATCHED BY SOURCE THEN DELETE;
```

## Expected Result

| ProductId | ProductName |
|---:|---|
| 1 | Laptop |
| 3 | Keyboard |
