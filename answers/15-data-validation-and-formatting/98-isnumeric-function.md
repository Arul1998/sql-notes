# Lesson 98 Answer: ISNUMERIC Function

## Exercise

Check whether `'125.50'` is numeric using `ISNUMERIC` and name the result `IsNumericValue`.

## Sample Table

| Value |
|---|
| 125.50 |

## Answer

```sql
SELECT ISNUMERIC('125.50') AS IsNumericValue;
```

## Expected Result

| IsNumericValue |
|---:|
| 1 |
