# Lesson 130: REPLICATE

`REPLICATE()` repeats a string the number of times you specify. You can use a column value as the repeat count.

## Sample Table

| ProductId | ProductName | StockLevel |
|---:|---|---:|
| 1 | Laptop | 4 |
| 2 | Mouse | 2 |
| 3 | Keyboard | 5 |
| 4 | Monitor | 3 |

## Syntax

```sql
REPLICATE(text, number_of_times)
```

## Example

```sql
SELECT REPLICATE('*', 3) AS Stars;
```

## Exercise

Using `Products`, display `ProductId`, `ProductName`, and `StockDisplay`. Use `REPLICATE()` to display one `#` for each unit in `StockLevel`.
