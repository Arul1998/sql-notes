# Lesson 83: GETUTCDATE Function

`GETUTCDATE` returns the current UTC date and time.

## Sample Table

Imagine this `Orders` table:

| OrderId | Amount |
|---:|---:|
| 101 | 125.20 |
| 102 | 250.75 |
| 103 | 399.10 |

## Syntax

```sql
GETUTCDATE()
```

## Example

```sql
SELECT GETUTCDATE() AS CurrentUTCDateTime;
```

## Exercise

Display `OrderId`, `Amount`, and the current UTC date and time.

Name the new column `UTCDateTime`.
