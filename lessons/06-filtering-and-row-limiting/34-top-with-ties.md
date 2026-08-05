# Lesson 34: TOP with TIES

`WITH TIES` includes extra rows that have the same final `ORDER BY` value as the last selected row.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 500 |
| 102 | 2 | 450 |
| 103 | 1 | 400 |
| 104 | 3 | 400 |
| 105 | 4 | 250 |

## Syntax

```sql
SELECT TOP (number) WITH TIES columns
FROM table_name
ORDER BY column_name;
```

## Example

```sql
SELECT TOP (2) WITH TIES *
FROM Orders
ORDER BY Amount DESC;
```

`WITH TIES` requires `ORDER BY`.

## Exercise

Display the top 3 orders by `Amount`, including tied rows.