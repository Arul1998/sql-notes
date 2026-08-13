# Lesson 96 Answer: TRY_CONVERT Function

## Exercise

Convert `'750'` to `INT` with `TRY_CONVERT` and name it `ConvertedNumber`.

## Sample Table

| Value |
|---|
| 750 |

## Answer

```sql
SELECT TRY_CONVERT(INT, '750') AS ConvertedNumber;
```

## Expected Result

| ConvertedNumber |
|---:|
| 750 |
