# Lesson 89 Answer: DATEFROMPARTS Function

## Exercise

Create the date `2026-12-25` using `DATEFROMPARTS` and name it `ChristmasDate`.

## Sample Table

No table is required.

| Year | Month | Day |
|---:|---:|---:|
| 2026 | 12 | 25 |

## Answer

```sql
SELECT DATEFROMPARTS(2026, 12, 25) AS ChristmasDate;
```

## Expected Result

| ChristmasDate |
|---|
| 2026-12-25 |
