# Lesson 118 Answer: TRY_CONVERT

## Exercise

Convert the text '2026-10-30' into a DATE using TRY_CONVERT.

## Sample Table

| Value |
|---|
| 2026-10-30 |

## Answer

```sql
SELECT TRY_CONVERT(DATE, '2026-10-30', 23) AS ConvertedDate;
```

## Expected Result

| ConvertedDate |
|---|
| 2026-10-30 |
