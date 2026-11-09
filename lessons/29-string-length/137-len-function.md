# Lesson 137: LEN

`LEN()` returns the number of characters in a string, excluding trailing spaces but including spaces between words.

## Sample Table

| CustomerId | CustomerName |
|---:|---|
| 1 | Arun |
| 2 | Priya |
| 3 | Christopher |
| 4 | James |

## Syntax

```sql
LEN(text)
```

## Example

```sql
SELECT LEN('SQL Server') AS TextLength;
```

## Exercise

Using `Customers`, display `CustomerId`, `CustomerName`, and `NameLength`. Use `LEN()` to count the characters in each customer name.
