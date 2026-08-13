# Lesson 97 Answer: ISDATE Function

## Exercise

Check whether `'2026-12-25'` is a valid date using `ISDATE` and name the result `IsValidDate`.

## Sample Table

| Value |
|---|
| 2026-12-25 |

## Answer

```sql
SELECT ISDATE('2026-12-25') AS IsValidDate;
```

## Expected Result

| IsValidDate |
|---:|
| 1 |
