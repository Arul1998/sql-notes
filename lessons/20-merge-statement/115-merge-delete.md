# Lesson 115: MERGE (DELETE Missing Rows)

`WHEN NOT MATCHED BY SOURCE` deletes target rows absent from the source.

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

## Syntax

```sql
MERGE target AS t USING source AS s ON t.Id = s.Id WHEN NOT MATCHED BY SOURCE THEN DELETE;
```

## Example

```sql
MERGE Products AS t
USING NewProducts AS s ON t.ProductId = s.ProductId
WHEN NOT MATCHED BY SOURCE THEN DELETE;
```

## Exercise

Delete products that do not appear in NewProducts.
