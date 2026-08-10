# Lesson 71 Answer: SPACE Function

## Exercise

Display a calculated column named `CustomerDetails`.

Use `CONCAT` and `SPACE` to join `CustomerName`, two spaces, and `City`.

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
SELECT CONCAT(CustomerName, SPACE(2), City) AS CustomerDetails
FROM Customers;
```

## Expected Result

### Result

| CustomerDetails |
|---|
| Sarah  London |
| David   |
| Priya  Chennai |
| James  Manchester |
| Amina  London |
