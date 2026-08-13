# Lesson 97: ISDATE Function

`ISDATE` checks whether SQL Server recognizes a value as a valid date or time.

It returns `1` for a valid value and `0` for an invalid value.

## Sample Table

No table is required for this lesson.

| Value |
|---|
| 2026-12-25 |

## Syntax

```sql
ISDATE(value)
```

## Example

```sql
SELECT ISDATE('2026-08-12') AS IsValidDate;
```

## Exercise

Check whether `'2026-12-25'` is a valid date using `ISDATE`.

Name the result `IsValidDate`.
