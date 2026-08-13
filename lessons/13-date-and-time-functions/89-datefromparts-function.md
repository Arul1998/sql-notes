# Lesson 89: DATEFROMPARTS Function

`DATEFROMPARTS` creates a date from separate year, month, and day values.

## Sample Table

No table is required for this lesson.

| Year | Month | Day |
|---:|---:|---:|
| 2026 | 8 | 10 |

## Syntax

```sql
DATEFROMPARTS(year, month, day)
```

## Example

```sql
SELECT DATEFROMPARTS(2026, 8, 10) AS CreatedDate;
```

## Exercise

Create the date `2026-12-25` using `DATEFROMPARTS`.

Name the result `ChristmasDate`.
