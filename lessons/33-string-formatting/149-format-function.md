# Lesson 149: FORMAT

`FORMAT()` converts numeric or date values into formatted text. The `C2` pattern formats currency with two decimal places; `en-GB` uses British pounds.

## Sample Table

| ProductId | ProductName | Price |
|---:|---|---:|
| 1 | Laptop | 1299.5 |
| 2 | Mouse | 25 |
| 3 | Keyboard | 79.99 |
| 4 | Monitor | 350.75 |

## Syntax

```sql
FORMAT(value, 'format_pattern', 'culture')
```

## Example

```sql
SELECT FORMAT(1234.5, 'C2', 'en-GB') AS FormattedPrice;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `FormattedPrice`. Use `FORMAT()` to show `Price` in British pounds with exactly two decimal places (`'C2'`, `'en-GB'`).
