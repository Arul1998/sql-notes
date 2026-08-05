# Lesson 26: Updating Multiple Columns

An `UPDATE` statement can change more than one column in the same row.

Separate each column and its new value with a comma inside the `SET` clause.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |

## Syntax

```sql
UPDATE table_name
SET column_name1 = new_value1,
    column_name2 = new_value2
WHERE condition;
```

## Examples

To change both the customer and amount for order 102:

```sql
UPDATE Orders
SET CustomerId = 3,
    Amount = 400
WHERE OrderId = 102;
```

You can update more columns by separating each assignment with a comma:

```sql
UPDATE Orders
SET CustomerId = 2,
    Amount = 300
WHERE OrderId = 105;
```

Always use a suitable `WHERE` condition when you only want to update a specific row.

## Exercise

Update order 103:

- Change `CustomerId` to 2.
- Change `Amount` to 275.
