# Lesson 143: SPACE

`SPACE()` generates the specified number of spaces. Combine it with `CONCAT()` when formatting text.

## Sample Table

| CustomerId | FirstName | LastName |
|---:|---|---|
| 1 | Arun | Kumar |
| 2 | Priya | Sharma |
| 3 | James | Brown |
| 4 | David | Wilson |

## Syntax

```sql
SPACE(number_of_spaces)
```

## Example

```sql
SELECT CONCAT('Hello', SPACE(3), 'SQL') AS Result;
```

## Exercise

Using `Customers`, display `CustomerId` and `CustomerFullName`. Use `CONCAT()` and `SPACE(3)` to place exactly three spaces between each `FirstName` and `LastName`.
