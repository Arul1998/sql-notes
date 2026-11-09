# Lesson 128: REPLACE

`REPLACE()` finds every occurrence of specified text and replaces it with new text in the result. A `SELECT` does not update the original data.

## Sample Table

| ProductId | ProductName | Category |
|---:|---|---|
| 1 | Apple iPhone | Mobile |
| 2 | Samsung Galaxy | Mobile |
| 3 | Dell Laptop | Computer |
| 4 | HP Laptop | Computer |

## Syntax

```sql
REPLACE(text, old_text, new_text)
```

## Example

```sql
SELECT REPLACE('Hello World', 'World', 'SQL') AS UpdatedText;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `UpdatedCategory`. Use `REPLACE()` to display `Smartphone` instead of `Mobile` in `Category`, without updating the table.
