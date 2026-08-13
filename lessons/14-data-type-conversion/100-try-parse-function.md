# Lesson 100: TRY_PARSE Function

`TRY_PARSE` tries to convert text into a specified data type.

If the conversion fails, it returns `NULL` instead of an error.

## Sample Table

No table is required for this lesson.

| Value |
|---|
| 500 |

## Syntax

```sql
TRY_PARSE(string_value AS data_type)
```

## Example

```sql
SELECT TRY_PARSE('125.50' AS DECIMAL(10,2)) AS Amount;
```

## Exercise

Convert `'500'` to `INT` using `TRY_PARSE`.

Name the result `ParsedNumber`.
