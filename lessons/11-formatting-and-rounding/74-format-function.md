# Lesson 74: FORMAT Function

`FORMAT` displays a number or date in a chosen format.

The format `N2` displays a number with two decimal places.

## Sample Table

Imagine this `Orders` table:

| OrderId | CustomerId | Amount |
|---:|---:|---:|
| 101 | 1 | 200.25 |
| 102 | 2 | 500.00 |
| 103 | 1 | 150.75 |
| 104 | 3 | 750.68 |
| 105 | 4 | 300.40 |

## Syntax

```sql
FORMAT(value, format)
```

## Example

```sql
SELECT OrderId,
       FORMAT(Amount, 'N1') AS FormattedAmount
FROM Orders;
```

## Exercise

Display `OrderId`, `Amount`, and `FormattedAmount`.

Use `FORMAT` with `N2` to show two decimal places.
