# Lesson 32: TOP with ORDER BY

Use `TOP` with `ORDER BY` when you need the highest or lowest rows.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |

## Syntax

```sql
SELECT TOP (number) columns
FROM table_name
ORDER BY column_name ASC | DESC;
```

## Example

```sql
SELECT TOP (2) *
FROM Orders
ORDER BY Amount DESC;
```

`ASC` returns the lowest values first. `DESC` returns the highest values first.

## Exercise

Display the 2 orders with the lowest `Amount`.