# Lesson 43: LIKE: Ends With

Place `%` before text to find values that end with that text.

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
WHERE column_name LIKE '%text';
```

## Example

```sql
SELECT *
FROM Customers
WHERE CustomerName LIKE '%a';
```

`'%a'` matches any text ending in a.

## Exercise

Display customers whose name ends with `n`.