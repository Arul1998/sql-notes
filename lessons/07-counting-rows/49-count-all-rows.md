# Lesson 49: Counting All Rows

`COUNT(*)` returns the total number of rows in a result.

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
SELECT COUNT(*)
FROM table_name;
```

## Example

```sql
SELECT COUNT(*)
FROM Orders;
```

`COUNT(*)` includes every row, even when some columns contain `NULL`.

## Exercise

Count all rows in the `Orders` table.