# Lesson 57 Answer: COALESCE Function

## Exercise

Display `CustomerName` and `ContactLocation` from `Customers`.

Return `City`, otherwise `Country`, otherwise `Unknown`.

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
       COALESCE(City, Country, 'Unknown') AS ContactLocation
FROM Customers;
```

## Expected Result

### Result

| CustomerName | ContactLocation |
|---|---|
| Sarah | London |
| David | UK |
| Priya | Chennai |
| James | Manchester |
| Amina | London |
