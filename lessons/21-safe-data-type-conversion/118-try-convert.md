# Lesson 118: TRY_CONVERT

`TRY_CONVERT` safely converts a value to another data type.

## Sample Table

| Value |
|---|
| 2026-10-30 |

## Syntax

```sql
TRY_CONVERT(data_type, expression [, style])
```

## Example

```sql
SELECT TRY_CONVERT(DATE, '2026-10-30', 23) AS ConvertedDate;
```

## Exercise

Convert the text '2026-10-30' into a DATE using TRY_CONVERT.
