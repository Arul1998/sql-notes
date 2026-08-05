# Lesson 45: LIKE: Single-Character Wildcard

In a `LIKE` pattern, `_` represents exactly one character.

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
WHERE column_name LIKE '_text';
```

## Example

```sql
SELECT *
FROM Customers
WHERE CustomerName LIKE '_ara';
```

`'_ara'` matches four-character values with any first character followed by ara.

## Exercise

Display customers whose name has any first character followed by `ohn`.