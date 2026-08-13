# Lesson 93: CAST Function

`CAST` converts a value from one data type to another.

## Sample Table

Imagine this `Orders` table:

| OrderId | Amount |
|---:|---:|
| 101 | 125.75 |
| 102 | 250.20 |

## Syntax

```sql
CAST(value AS data_type)
```

## Example

```sql
SELECT OrderId,
       CAST(Amount AS INT) AS WholeAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and convert `Amount` to `INT`.

Name the new column `IntegerAmount`.
