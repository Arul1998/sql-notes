# Lesson 95: TRY_CAST Function

`TRY_CAST` tries to convert a value to another data type.

If the conversion fails, it returns `NULL` instead of a conversion error.

## Sample Table

No table is required for this lesson.

| Value |
|---|
| 250 |

## Syntax

```sql
TRY_CAST(value AS data_type)
```

## Example

```sql
SELECT TRY_CAST('123' AS INT) AS Number;
```

## Exercise

Convert `'250'` to `INT` using `TRY_CAST`.

Name the result `ConvertedNumber`.
