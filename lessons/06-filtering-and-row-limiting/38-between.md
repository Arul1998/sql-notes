# Lesson 38: Filtering with BETWEEN

`BETWEEN` checks whether a value is inside an inclusive range.

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
SELECT columns
FROM table_name
WHERE column_name BETWEEN lower_value AND upper_value;
```

## Example

```sql
SELECT *
FROM Orders
WHERE Amount BETWEEN 200 AND 500;
```

Both boundary values are included.

## Exercise

Display orders with an `Amount` between 250 and 400.