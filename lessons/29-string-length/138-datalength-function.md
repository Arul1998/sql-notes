# Lesson 138: DATALENGTH

`DATALENGTH()` counts the number of bytes used to represent a value, including trailing spaces. For basic English characters, `NVARCHAR` uses two bytes per character.

## Sample Table

`CustomerName` has data type `NVARCHAR(50)`.

| CustomerId | CustomerName |
|---:|---|
| 1 | Arun |
| 2 | Priya |
| 3 | Christopher |
| 4 | James |

## Syntax

```sql
DATALENGTH(expression)
```

## Example

```sql
SELECT DATALENGTH(N'Hello') AS UnicodeByteCount;
```

## Exercise

Using `Customers`, display `CustomerId`, `CustomerName`, and `NameBytes`. Use `DATALENGTH()` to count the bytes in each `NVARCHAR(50)` customer name.
