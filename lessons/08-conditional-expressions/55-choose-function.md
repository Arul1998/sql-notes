# Lesson 55: CHOOSE Function

`CHOOSE` returns an item from a list based on its numeric position.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 500 |
| 103 | 1 | 150 |
| 104 | 3 | 750 |
| 105 | 4 | 300 |

## Syntax

```sql
CHOOSE(index_number, value1, value2, value3)
```

## Example

```sql
SELECT OrderId,
       CHOOSE(2, 'Standard', 'Express', 'Collection') AS DeliveryType
FROM Orders;
```

## Exercise

Display `OrderId` and `DeliveryType` from `Orders`.

Use `CHOOSE(1, 'Standard', 'Express', 'Collection')`.
