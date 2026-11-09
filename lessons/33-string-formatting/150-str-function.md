# Lesson 150: STR

`STR()` converts a number into a `VARCHAR` string with a chosen width and decimal precision. It can add leading spaces; `LTRIM()` removes them.

## Sample Table

| OrderId | CustomerName | TotalAmount |
|---:|---|---:|
| 101 | Arun | 1500.456 |
| 102 | Priya | 250.5 |
| 103 | James | 75.999 |
| 104 | Sarah | 3200.125 |

## Syntax

```sql
STR(number, total_length, decimal_places)
```

## Example

```sql
SELECT LTRIM(STR(123.456, 8, 2)) AS AmountText;
```

## Exercise

Using `Orders`, display `OrderId`, `CustomerName`, and `AmountText`. Use `STR(TotalAmount, 10, 2)` and `LTRIM()` to show each amount as text with two decimal places and no leading spaces.
