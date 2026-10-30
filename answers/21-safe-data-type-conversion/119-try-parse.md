# Lesson 119 Answer: TRY_PARSE

## Exercise

Convert '125.50' into DECIMAL(10,2) using TRY_PARSE.

## Sample Table

| Value |
|---|
| 125.50 |

## Answer

```sql
SELECT TRY_PARSE('125.50' AS DECIMAL(10,2)
USING 'en-US') AS ParsedAmount;
```

## Expected Result

| ParsedAmount |
|---:|
| 125.50 |
