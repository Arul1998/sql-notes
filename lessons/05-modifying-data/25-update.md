# Lesson 25: UPDATE

`UPDATE` changes existing data in a table.

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200 |
| 102 | 2 | 350 |
| 103 | 1 | 150 |
| 104 | 3 | 500 |
| 105 | 4 | 250 |

To change the amount of order 105:

```sql
UPDATE Orders
SET Amount = 300
WHERE OrderId = 105;
```

- `UPDATE` specifies the table.
- `SET` specifies the new value.
- `WHERE` identifies the row to change.

Always check the `WHERE` condition. Without it, every row will be updated:

```sql
UPDATE Orders
SET Amount = 300;
```

SQL generally follows this pattern:

```sql
UPDATE table_name
SET column_name = new_value
WHERE condition;
```

## Exercise

Change the amount of order 102 to 400.
