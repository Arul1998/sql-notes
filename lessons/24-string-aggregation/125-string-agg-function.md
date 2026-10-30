# Lesson 125: STRING_AGG

`STRING_AGG` combines values from multiple rows into one string. The order is not guaranteed unless specified.

## Sample Table

| OrderId | CustomerId | ProductName |
|---:|---:|---|
| 101 | 1 | Laptop |
| 102 | 1 | Mouse |
| 103 | 2 | Keyboard |
| 104 | 2 | Monitor |

## Syntax

```sql
STRING_AGG(expression, separator)
```

## Example

```sql
SELECT CustomerId, STRING_AGG(ProductName, ', ') AS Products
FROM Orders
GROUP BY CustomerId;
```

## Exercise

Return CustomerId and Products. Combine product names for each customer using ', ' as the separator.
