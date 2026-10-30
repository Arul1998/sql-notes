# Lesson 114 Answer: MERGE (INSERT and UPDATE)

## Exercise

Update matching products and insert missing products from NewProducts.

## Sample Tables

**Products**

| ProductId | ProductName | Price |
|---:|---|---:|
| 1 | Laptop | 800 |
| 2 | Mouse | 20 |

**NewProducts**

| ProductId | ProductName | Price |
|---:|---|---:|
| 2 | Mouse | 25 |
| 3 | Keyboard | 50 |

## Answer

```sql
MERGE Products AS t
USING NewProducts AS s ON t.ProductId = s.ProductId
WHEN MATCHED THEN UPDATE SET t.Price = s.Price
WHEN NOT MATCHED BY TARGET THEN INSERT (ProductId, ProductName, Price) VALUES (s.ProductId, s.ProductName, s.Price);
```

## Expected Result

| ProductId | ProductName | Price |
|---:|---|---:|
| 1 | Laptop | 800 |
| 2 | Mouse | 25 |
| 3 | Keyboard | 50 |
