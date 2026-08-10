# Lesson 60 Answer: CONCAT_WS Function

## Exercise

Display `CustomerName`, `City`, `Country`, and `FullLocation`.

Join the three values with a comma followed by a space.

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
       Country,
       CONCAT_WS(', ', CustomerName, City, Country) AS FullLocation
FROM Customers;
```

## Expected Result

### Result

| CustomerName | City | Country | FullLocation |
|---|---|---|---|
| Sarah | London | UK | Sarah, London, UK |
| David | NULL | UK | David, UK |
| Priya | Chennai | India | Priya, Chennai, India |
| James | Manchester | NULL | James, Manchester |
| Amina | London | UK | Amina, London, UK |
