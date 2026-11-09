# Lesson 131: STUFF

`STUFF()` removes a specified number of characters starting at a position, then inserts replacement text. SQL Server string positions start at 1.

## Sample Table

| ProductId | ProductName | ProductCode |
|---:|---|---|
| 1 | Laptop | PRD-1001 |
| 2 | Mouse | PRD-1002 |
| 3 | Keyboard | PRD-1003 |
| 4 | Monitor | PRD-1004 |

## Syntax

```sql
STUFF(text, start_position, number_to_remove, replacement_text)
```

## Example

```sql
SELECT STUFF('Hello World', 7, 5, 'SQL') AS UpdatedText;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `UpdatedProductCode`. Replace the first three characters (`PRD`) of each `ProductCode` with `ITEM`, preserving the hyphen.
