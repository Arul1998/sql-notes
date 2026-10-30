# Lesson 117 Answer: TRY_CAST

## Exercise

Convert '100', 'abc', and '250' into integers using TRY_CAST.

## Sample Table

| Value |
|---|
| 100 |
| abc |
| 250 |

## Answer

```sql
SELECT TRY_CAST(Value AS INT) AS ConvertedNumber
FROM (VALUES ('100'), ('abc'), ('250')) AS Numbers(Value);
```

## Expected Result

| ConvertedNumber |
|---:|
| 100 |
| NULL |
| 250 |
