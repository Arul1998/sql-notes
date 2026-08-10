# Lesson 56 Answer: ISNULL Function

## Exercise

Display `CustomerName`, `City`, and `DisplayCity` from `Customers`.

If `City` is `NULL`, display `Unknown`. Otherwise, display the original city.

## Sample Table

| CustomerId | CustomerName | City | Country |
|---:|---|---|---|
| 1 | Sarah | London | UK |
| 2 | David | NULL | UK |
| 3 | Priya | Chennai | India |
| 4 | James | Manchester | NULL |
| 5 | Amina | London | UK |

## Answer

```sql
SELECT CustomerName,
       City,
       ISNULL(City, 'Unknown') AS DisplayCity
FROM Customers;
```

## Expected Result

### Result

| CustomerName | City | DisplayCity |
|---|---|---|
| Sarah | London | London |
| David | NULL | Unknown |
| Priya | Chennai | Chennai |
| James | Manchester | Manchester |
| Amina | London | London |
