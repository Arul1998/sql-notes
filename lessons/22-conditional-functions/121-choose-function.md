# Lesson 121: CHOOSE

`CHOOSE` returns a value at a given 1-based position.

## Sample Table

| Position | Value |
|---:|---|
| 1 | Pending |
| 2 | Shipped |
| 3 | Delivered |

## Syntax

```sql
CHOOSE(index, value1, value2, ...)
```

## Example

```sql
SELECT CHOOSE(2, 'Pending', 'Shipped', 'Delivered') AS OrderStatus;
```

## Exercise

Use CHOOSE to return the second value from 'Pending', 'Shipped', 'Delivered'.
