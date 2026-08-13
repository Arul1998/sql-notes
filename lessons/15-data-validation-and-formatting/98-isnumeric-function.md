# Lesson 98: ISNUMERIC Function

`ISNUMERIC` checks whether SQL Server considers a value numeric.

## Sample Table

| Value |
|---|
| 125.50 |

## Syntax

```sql
ISNUMERIC(value)
```

## Example

```sql
SELECT ISNUMERIC('250') AS IsNumber;
```

## Exercise

Check whether `'125.50'` is numeric and name the result `IsNumericValue`.
