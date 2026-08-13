# Lesson 94: CONVERT Function

`CONVERT` changes a value from one data type to another.

## Sample Table

Imagine this `Orders` table:

| OrderId | Amount |
|---:|---:|
| 101 | 125.75 |
| 102 | 250.20 |

## Syntax

```sql
CONVERT(data_type, value)
```

## Example

```sql
SELECT OrderId,
       CONVERT(INT, Amount) AS IntegerAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and convert `Amount` to `INT` using `CONVERT`.

Name the new column `WholeAmount`.
