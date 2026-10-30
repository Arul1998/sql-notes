# Lesson 114: MERGE (INSERT and UPDATE)

`MERGE` can update matching rows and insert missing rows.

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

## Syntax

```sql
MERGE target AS t USING source AS s ON t.Id = s.Id WHEN MATCHED THEN UPDATE SET t.Value = s.Value WHEN NOT MATCHED BY TARGET THEN INSERT (Id, Value) VALUES (s.Id, s.Value);
```

## Example

```sql
MERGE Products AS t
USING NewProducts AS s ON t.ProductId = s.ProductId
WHEN MATCHED THEN UPDATE SET t.Price = s.Price
WHEN NOT MATCHED BY TARGET THEN INSERT (ProductId, ProductName, Price) VALUES (s.ProductId, s.ProductName, s.Price);
```

## Exercise

Update matching products and insert missing products from NewProducts.
