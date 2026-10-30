# Lesson 117: TRY_CAST

`TRY_CAST` returns NULL when conversion fails.

## Sample Table

| Value |
|---|
| 100 |
| abc |
| 250 |

## Syntax

```sql
TRY_CAST(expression AS data_type)
```

## Example

```sql
SELECT TRY_CAST(Value AS INT) AS ConvertedNumber
FROM (VALUES ('100'), ('abc'), ('250')) AS Numbers(Value);
```

## Exercise

Convert '100', 'abc', and '250' into integers using TRY_CAST.
