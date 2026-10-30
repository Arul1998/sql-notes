# Lesson 121 Answer: CHOOSE

## Exercise

Use CHOOSE to return the second value from 'Pending', 'Shipped', 'Delivered'.

## Sample Table

| Position | Value |
|---:|---|
| 1 | Pending |
| 2 | Shipped |
| 3 | Delivered |

## Answer

```sql
SELECT CHOOSE(2, 'Pending', 'Shipped', 'Delivered') AS OrderStatus;
```

## Expected Result

| OrderStatus |
|---|
| Shipped |
