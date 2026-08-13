# Lesson 100 Answer: TRY_PARSE Function

## Exercise

Convert `'500'` to `INT` using `TRY_PARSE` and name the result `ParsedNumber`.

## Sample Table

| Value |
|---|
| 500 |

## Answer

```sql
SELECT TRY_PARSE('500' AS INT) AS ParsedNumber;
```

## Expected Result

| ParsedNumber |
|---:|
| 500 |
