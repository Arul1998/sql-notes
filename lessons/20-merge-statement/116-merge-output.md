# Lesson 116: MERGE with OUTPUT

`MERGE OUTPUT` reports INSERT, UPDATE, or DELETE actions.

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
MERGE target AS t USING source AS s ON t.Id = s.Id WHEN MATCHED THEN UPDATE SET t.Value = s.Value WHEN NOT MATCHED BY TARGET THEN INSERT (Id, Value) VALUES (s.Id, s.Value) OUTPUT $action, INSERTED.Id;
```

## Example

```sql
MERGE Products AS t
USING NewProducts AS s ON t.ProductId = s.ProductId
WHEN MATCHED THEN UPDATE SET t.Price = s.Price
WHEN NOT MATCHED BY TARGET THEN INSERT (ProductId, ProductName, Price) VALUES (s.ProductId, s.ProductName, s.Price)
OUTPUT $action AS ActionTaken, INSERTED.ProductId AS ProductId;
```

## Exercise

Update matching product prices, insert new products and show the action for each affected product.
