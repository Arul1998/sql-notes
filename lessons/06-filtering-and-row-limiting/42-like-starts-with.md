# Lesson 42: LIKE: Starts With

In a `LIKE` pattern, `%` represents zero or more characters.

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
WHERE column_name LIKE 'text%';
```

## Example

```sql
SELECT *
FROM Customers
WHERE CustomerName LIKE 'S%';
```

`'S%'` matches text that starts with S.

## Exercise

Display customers whose name starts with `M`.