# Lesson 39: Filtering with NOT BETWEEN

`NOT BETWEEN` returns values outside an inclusive range.

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
WHERE column_name NOT BETWEEN lower_value AND upper_value;
```

## Example

```sql
SELECT *
FROM Orders
WHERE Amount NOT BETWEEN 100 AND 300;
```

Values equal to either boundary are excluded from the result.

## Exercise

Display orders whose `Amount` is not between 200 and 400.