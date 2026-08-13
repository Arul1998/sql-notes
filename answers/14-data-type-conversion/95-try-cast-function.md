# Lesson 95 Answer: TRY_CAST Function

## Exercise

Convert `'250'` to `INT` using `TRY_CAST` and name the result `ConvertedNumber`.

## Sample Table

No table is required.

| Value |
|---|
| 250 |

## Answer

```sql
SELECT TRY_CAST('250' AS INT) AS ConvertedNumber;
```

## Expected Result

| ConvertedNumber |
|---:|
| 250 |
