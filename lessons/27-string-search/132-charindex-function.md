# Lesson 132: CHARINDEX

`CHARINDEX()` returns the starting position of the first exact text match. Positions start at 1; it returns 0 if there is no match.

## Sample Table

| ProductId | ProductCode |
|---:|---|
| 1 | LAP-1001 |
| 2 | MOU-2002 |
| 3 | KEY-3003 |
| 4 | MON-4004 |

## Syntax

```sql
CHARINDEX(text_to_find, text_to_search)
```

## Example

```sql
SELECT CHARINDEX('@', 'john@gmail.com') AS AtPosition;
```

## Exercise

Using `Products`, display `ProductId`, `ProductCode`, and `HyphenPosition`. Use `CHARINDEX()` to find the position of `-` in each `ProductCode`.
