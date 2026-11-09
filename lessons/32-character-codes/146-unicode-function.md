# Lesson 146: UNICODE

`UNICODE()` returns the Unicode numeric value of the first character in a string. Unicode supports international scripts, including Tamil.

## Sample Table

`CustomerName` is `NVARCHAR(100)`.

| CustomerId | CustomerName |
|---:|---|
| 1 | Alice |
| 2 | Bob |
| 3 | Charlie |
| 4 | David |

## Syntax

```sql
UNICODE(text)
```

## Example

```sql
SELECT UNICODE(N'த') AS UnicodeValue;
```

## Exercise

Using `Customers`, display `CustomerId`, `CustomerName`, and `FirstCharacterUnicode`. Use `UNICODE()` to find the Unicode value of the first character of each `CustomerName`.
