# Lesson 28: Deleting a Specific Row

The `DELETE` statement removes rows from a table. Use a `WHERE` condition when you want to remove only one specific row.

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
DELETE FROM table_name
WHERE condition;
```

## Example

```sql
DELETE FROM Orders
WHERE OrderId = 105;
```

Before running `DELETE`, check the `WHERE` condition carefully.

## Exercise

Delete the order whose `OrderId` is 101.