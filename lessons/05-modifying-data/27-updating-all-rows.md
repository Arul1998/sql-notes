# Lesson 27: Updating All Rows

An `UPDATE` statement without a `WHERE` clause changes every row in the table.

## Sample Table

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |

## Syntax

```sql
UPDATE table_name
SET column_name = new_value;
```

## Examples

```sql
UPDATE Orders
SET Amount = 500;
```

This changes the `Amount` value to 500 for every order.

Always check whether you need a `WHERE` clause before running an `UPDATE` statement.

## Exercise

Update all orders so that `Amount` becomes 500.
