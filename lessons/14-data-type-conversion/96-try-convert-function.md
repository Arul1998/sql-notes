# Lesson 96: TRY_CONVERT Function

`TRY_CONVERT` tries to convert a value to another data type.

If conversion fails, it returns `NULL` instead of a conversion error.

## Sample Table

No table is required for this lesson.

| Value |
|---|
| 750 |

## Syntax

```sql
TRY_CONVERT(data_type, value)
```

## Example

```sql
SELECT TRY_CONVERT(INT, '500') AS Number;
```

## Exercise

Convert `'750'` to `INT` using `TRY_CONVERT`.

Name the result `ConvertedNumber`.
