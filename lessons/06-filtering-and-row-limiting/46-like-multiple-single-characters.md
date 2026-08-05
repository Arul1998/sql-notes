# Lesson 46: LIKE: Multiple Single-Character Wildcards

Use more than one `_` when a pattern needs multiple exact character positions.

## Sample Table

| CustomerId | CustomerName | City |
|---:|---|---|
| 1 | Arul | London |
| 2 | Priya | Manchester |
| 3 | John | London |
| 4 | Sara | Birmingham |
| 5 | Maya | Manchester |

## Syntax

```sql
SELECT columns
FROM table_name
WHERE column_name LIKE '__text';
```

## Example

```sql
SELECT *
FROM Customers
WHERE CustomerName LIKE '__ra';
```

Each underscore represents exactly one character.

## Exercise

Display customers whose name has two characters followed by `ya`.