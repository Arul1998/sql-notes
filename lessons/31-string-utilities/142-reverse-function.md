# Lesson 142: REVERSE

`REVERSE()` returns a string with its characters in reverse order. A `SELECT` does not change the stored value.

## Sample Table

| ProductId | ProductCode |
|---:|---|
| 1 | LAP100 |
| 2 | MOU200 |
| 3 | KEY300 |
| 4 | MON400 |

## Syntax

```sql
REVERSE(text)
```

## Example

```sql
SELECT REVERSE('SQL') AS ReversedText;
```

## Exercise

Using `Products`, display `ProductId`, `ProductCode`, and `ReversedProductCode`. Use `REVERSE()` to reverse every character of `ProductCode`.
