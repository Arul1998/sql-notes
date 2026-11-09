# Lesson 133: PATINDEX

`PATINDEX()` returns the starting position of the first text pattern matching a wildcard expression. It returns 0 if no match is found.

## Sample Table

| ProductId | ProductCode |
|---:|---|
| 1 | LAP1001 |
| 2 | MOUSE202 |
| 3 | KEY45 |
| 4 | MONITOR789 |

## Syntax

```sql
PATINDEX('%pattern%', text_to_search)
```

## Example

```sql
SELECT PATINDEX('%[0-9]%', 'ABC123') AS FirstDigitPosition;
```

## Exercise

Using `Products`, display `ProductId`, `ProductCode`, and `FirstNumberPosition`. Use `PATINDEX()` to find the position of the first digit (`0`–`9`) in each `ProductCode`.
